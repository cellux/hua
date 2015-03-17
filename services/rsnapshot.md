# rsnapshot

* backups stored under `/backup/{hourly,daily,weekly,monthly}.[0-9]*/
* must run once every hour/day/week/month to make the backups
* a lockfile is created and locked while rsnapshot is running to ensure only one instance is running at a time

## Implements

* `backup`

## Files

* binary: `/usr/bin/rsnapshot`
* configuration: `/etc/rsnapshot.conf`
* log: /var/log/rsnapshot.log
* cron job: `/etc/cron.d/rsnapshot`
* lock file: `/var/run/rsnapshot.pid`

## Configuration

* `snapshot_root`: the root directory of backups (`/backup`)
* `logfile`: Path to log
* `exclude`: patterns to exclude
* `lockfile`: where to keep the lock file
* `backup` <path> <target>
* `backup_script` <script> <target>
