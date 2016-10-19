snapes or Snap_ES
Creates and maintains a set number of Elastic Search repository snapshots in some repository

https://www.elastic.co/guide/en/elasticsearch/reference/current/modules-snapshots.html
Put this script in cron and run at desired frequency
Before starting this script you must ensure that the repo is setup and the es host has read/write access to the repo.
It is usually run out of either /etc/crontab or a user cron as follows, pick your time of day (these are based on UTC)

01 10,22 * * * /usr/local/bin/snapes > /var/log/search-backup.log 2>&1

Depends on having 
jq installed from https://stedolan.github.io/jq/

references
http://tech.rhealitycheck.com/elasticsearch-snapshots-and-restore-on-aws-s3/
https://github.com/elastic/elasticsearch-cloud-aws
https://github.com/elastic/elasticsearch-cloud-aws/tree/v2.3.0#version-230-for-elasticsearch-13