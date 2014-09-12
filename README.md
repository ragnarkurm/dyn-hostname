This script goes to
/etc/init/hostname-by-lookup.conf

On reboot it resolves current IP to FQDN,
extracts portion before first dot,
puts it into /etc/hostname
and sets current hostname.

Example, your IP resoves to jim-workstation-02.example.com
the script extracts jim-workstation-02 and puts to
/etc/hostname and sets current hostname.

This script is useful to control set of hosts
which have IP addresses and names set by dynamically by DHCP.

This script is automatically run on startup by Upstart
http://upstart.ubuntu.com/getting-started.html
