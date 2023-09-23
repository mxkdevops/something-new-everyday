#!/bin/bash

# Destination directory for the backup
backup_dir="/home/vagrant/"

# backup filename
backup_filename="website"

#source directory to backup up
source_dir="/srv/www/"

#Number of days to keep old backups

days_to_keep=5

#Find and delete older than the specified days

find "$backup_dir" -name "${backup_filename}*.tar.gz" -type f -mtime +$days_to_keep -exec rm {} \;

#Create a compressed archive of the source directory
tar zcvf "$backup_dir/$backup_filename -$(date +%Y-%m-%d\ %H:%M:%S)".tar.gz -C "$source_dir" .

#Print a message indicating the backup is complete

echo " Backup of $source_dir completed at $(date +%Y-%m-%d\ %H:%M:%S)"
