# gcp-snapshots
Bash script to create daily snapshots using GoogleCloud API

How to use script:

1. Install Google Cloud SDK on some instance in the project

curl https://sdk.cloud.google.com | bash

gcloud init

2. Create dir and copy script to dir

3. Add cronjob to run script for example daily at 3 AM (and also log results of script execution)

0 3 * * * bash /opt/gcp-snapshots/gcps.sh >> /var/log/cron/gcps.log 2>&1

4. Enjoy automated snapshots creation for all existing and new disks in project
