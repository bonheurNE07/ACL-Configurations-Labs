**R2**

g0/0

1. deny 192.168.11.0/24 to access 192.168.20.254 out
2. permit any out



**commands**



*access-list 1 deny 192.168.11.0 0.0.0.255*

*access-list 1 permit any*



*config) # interface g0/0*

*config-if)#ip access-group 1 out*







R3

g0/0

1. deny 192.168.10.0/24 to access 192.168.30.0/24 out out
2. prmit any out



**commands**



*access-list 1 deny 192.168.10.0 0.0.0.255*

*access-list 1 permit any*



*config) # interface g0/0*

*config-if)#ip access-group 1 out*







