# pan_dhcp

This is a python script that pulls client information from the DHCP service associated with every interface on a Palo Alto Networks firewall
and populates the hostname (if available) and MAC address into the User-ID registration on the firewall allowing this information to be
populated in all log events as well as allowing new rules to be created based on these user IDs.

The power of this is to move away from statically assigning IP addresses or creating DHCP reservations for every device to enable writing specific
security rules for those devices.  This script allows you to write the rule using the user-ID and the rule will follow the system regardless of
the IP address it is assigned by the DHCP service.
