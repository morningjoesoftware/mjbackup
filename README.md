# MJBackup - Morning Joe Software Linux Server Backup System.

This script is called to perform a backup and in turn calls other scripts which perform
specialized task such as back up files, MySql databases, Postgresql databases, and anything
else that this can be extended to support.

The files are archived with a time/date timestamp and multiple copies of a backup are supported.
Appending the status to the logfile /var/log/mjbackup/mjbackup.log is supported.
Automatically emailing the status of the backup/log is supported.  The number of backups retained
can be limited and set in the configuration files.

There is also a script that can be used to rsync the backup files to the remote location.  The length
these remote copies can be retained can be set by days.

Both scripts are meant to be used with crontab in a linux server environment.