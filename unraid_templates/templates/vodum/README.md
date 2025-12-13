# VODUM

VODUM is a VOD user subscription manager designed for Unraid.

## Features
- User & subscription management
- SQLite database (persistent)
- Automated expiration handling
- Web-based interface
- Lightweight & Unraid-friendly

## Default Configuration
- Web UI: http://[IP]:5000
- Appdata path: /mnt/user/appdata/vodum

## Volumes
| Container Path | Host Path |
|---------------|----------|
| /appdata | /mnt/user/appdata/vodum |
| /logs | /mnt/user/appdata/vodum/logs |
| /backups | /mnt/user/appdata/vodum/backups |

## Notes
- SQLite database stored in `/appdata/database.db`
- No Plex or Jellyfin token required at container level
