snapes or Snap_ES
Creates and maintains a set number of Elastic Search repository snapshots in some repository

https://www.elastic.co/guide/en/elasticsearch/reference/current/modules-snapshots.html
Put this script in cron and run at desired frequency
Before starting this script you must ensure that the repo is setup and the es host has read/write access to the repo.

Depends on having 
jq installed from https://stedolan.github.io/jq/
http://tech.rhealitycheck.com/elasticsearch-snapshots-and-restore-on-aws-s3/
https://github.com/elastic/elasticsearch-cloud-aws