# SELKS-probe
SELKS probe for Azure

Options:
-daemonlogger
-rpcap
-Suricata

Add ansible scripts to reboot/update probes.


# Setup Azure file share storage

First thing we need to do is setup the storage area for all of our pcap or json files.  Later we will use filebeat and connect to the file share storage and ship those files to logstash for processing into elasticsearch.

Follow this how-to from Microsoft:

https://docs.microsoft.com/en-us/azure/storage/files/storage-how-to-create-file-share



# Setup Suricata on host to monitor

-Add info

-Add how to mount to Azure blob storage

-Add configurations



# Setup Filebeat Server

-Add info

-Add how to mount to blob storage

-Add configurations
