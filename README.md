# logwall
logwall for syslog is an analogue to firewall for IP networks. 
many distributors set /dev/log socket world-writable, 
this may cause enfake of the system logs on multiuser systems. 
one solution to set 660 as file mode and sort users and their processes into unix groups 
by which it's allowed or denied to access /dev/log for write. 

logwall gives more flexibility to control who be able to log 
in which facility and at which priority 
with a ruleset based on peer socket properties.
