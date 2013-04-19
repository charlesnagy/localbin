localbin
========

Useful /usr/local/bin scripts for very different purposes

## Install ##

	sudo make install

## Scripts ##

### ftp_share ###
Very simple helper script for managing PureFTPd shares with PostgreSQL auth backend.

	Usage: ftp_share [options] path

	Options:
	  -h, --help            show this help message and exit
	  -l, --list            List all shares
	  -u USERNAME, --user=USERNAME
							FTP username
	  -d DOWNLOAD_LIMIT, --download-limit=DOWNLOAD_LIMIT
							Download bandwith limit

If list option enabled path will be used for quering the dataset. 
If creating new share path will be the basedirectory.

### backup_mysql ###
Wrapper around Percona Xtrabackup

	Usage: backup_mysql [options]

	Options:
	  -h, --help            show this help message and exit
      -d BACKUPDIR, --backupdir=BACKUPDIR
	                        Backup base directory
	  -r RETENTION, --retention=RETENTION
	                        Number of days how long the backup should be kept

Backupdir option is mandatory.

Example:

	backup_mysql -d /backups/mysql

You can find me on [Twitter](https://twitter.com/charlesnagy "Charlesnagy Twitter"), [My Blog](http://charlesnagy.info/ "Charlesnagy.info") or [LinkedIn]("http://www.linkedin.com/in/nkaroly" "Károly Nagy - MySQL DBA")
