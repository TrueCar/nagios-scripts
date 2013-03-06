nagios-scripts
==============

Collection of various Nagios scripts

### check_kafka_lag.sh

Used to check the lag between to Kafka instnaces, one used as a "producer" and
the other as a "consumer". Don't know if it's really useful outside my company 
but anyway, here it is

### check_graphite.sh

I know that there are at least two other projects here on GitHub for the same
purpose but they are both written in Ruby and I've developed an idiosincrasy
towards that language, as a sysadmin (I won't rant here :P).
Moreover, both of them are not flexible enough, cause I need dates range 
support and different calculation modes (they just return the last valid 
value). So here it is this simple bash script to check if a Graphite series
is within two given thresholds.
Check the program help for the options available

This script has a dependency on JSON.sh, you can find this great bash script 
here: https://github.com/dominictarr/JSON.sh

### check_ndb 

Previously in a separate repo, it is a scripts to monitor MySQL NDB Cluster from 
Nagios. It connects to the NDB Manager and check the memory used by the cluster
for the specified node

