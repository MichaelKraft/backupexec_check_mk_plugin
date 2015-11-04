# Backup Exec Nagios Plugin

Based on [Backup Exec plugin for check_mk](http://www.pawelko.net/backup-exec-plugin-for-check_mk/).

This version checks all active jobs, and then checks all non-successful jobs for active alerts in backup exec. In this way once you dismiss the alerts in backup exec they are cleared from Nagios as well.

Works by querying the table that handles the active alerts in Backup Exec and checking for the existence of a job with the same timestamp as an alert.

Verfied to work on Windows Server 2008 with Backup Exec 2012.