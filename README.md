
# Setup Azure file share storage

First thing we need to do is setup the storage area for all of our pcap or json files.  Later we will use filebeat and connect to the file share storage and ship those files to logstash for processing into elasticsearch.

Follow this how-to from Microsoft:

https://docs.microsoft.com/en-us/azure/storage/files/storage-how-to-create-file-share

# Setup Filebeat Server


-Add how to mount to file share storage

MORE TO COME:
https://www.elastic.co/guide/en/beats/filebeat/current/filebeat-installation.html

Configure filebeat.yml with this following information: 

( I will add my configs later, basically point it to SELKS logstash server for processing and configure the SMB3 file share paths.  These paths will be determined during your mounting step to the file share in Azure )

-Add configurations examples to collect all logs and push to SELKS logstash.

# SELKS-probe

SELKS probe for Azure (depends on level of detail, more to come)

Options:
-daemonlogger
-rpcap
-Suricata 

Add ansible scripts to reboot/update probes.

Quick and dirty, more to come:

In a nutshell: Install a lightweight server (CentOS or Ubuntu), this is required because of the SMB3 requirements. Currently SELKS is built on Debian 9 but the kernal at this time, does not support SMB3.

After you have install the Linux OS, install Suricata(CentOs or Ubuntu):

https://www.howtoforge.com/tutorial/suricata-with-elk-and-web-front-ends-on-ubuntu-bionic-beaver-1804-lts/

Copy SELKS Suricata.yml file from SELKS install.  Change logging paths to reflect file share within Azure. Mount SMB3 file share. (More details to come)



# Setup Suricata on host to monitor

-Add info about installing Suricata as a probe (pcap or meta data only or both)

-Add how to mount to Azure file share storage and dump all files to the file share.

-Add configuration files




