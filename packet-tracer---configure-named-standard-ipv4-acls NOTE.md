**R1**



only **host** 192.168.20.4/24(manager host\[pc]) and **host** 192.168.100.100/24(web server) should be able to access the 192.168.20.1/24 (file server) **on** R3 *interface fa0/1* 



<b>commands</b>



*ip access-list standard FileServerRestrictions*

*permit host 192.168.20.4*

*permit 192.168.100.100*

*deny any*



*interface fa0/1*

*ip access-group FileServerRestrictions out*

