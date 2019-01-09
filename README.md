# findilos
Search a local network segment for iLOs
The iLO is the Integrated Lights-Out management processor
used on HP ProLiant and BladeSystem servers

Original Author: iggy@nachotech.com

Requires: tr sed expr curl nmap

Tested with: Nmap 4.20, curl 7.17.1, RHEL4

# Note:
Discovery of an iLO is dependent upon the Virtual Media port
being set to the default of 17988.  If this has been changed
by the iLO administrator, then this script will NOT find it.

Also, if the iLO XML Reply Data Return has been Disabled by
the iLO administrator, this script will not be able to
gather any information about the server.  It will still be
discovered, but all you will see is its IP address.
