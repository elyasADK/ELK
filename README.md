# logstash-mikrotik-cisco and more...
how to connect logstash to mikrotik, Cisco and more...

This is ELK with Mikrotik, Cisco and more...

*DONT FORGET TO CHANGE PASSWORD IN ALL FILES*

DONT FORGET : give permission to your directory (elasticsearch - kibana - logstash)




Virtual memoryedit
Elasticsearch uses a mmapfs directory by default to store its indices. The default operating system limits on mmap counts is likely to be too low, which may result in out of memory exceptions.

On Linux, you can increase the limits by running the following command as root:

sysctl -w vm.max_map_count=262144

To set this value permanently, update the vm.max_map_count setting in /etc/sysctl.conf. To verify after rebooting, run sysctl vm.max_map_count.

The RPM and Debian packages will configure this setting automatically. No further configuration is required.


