**ROUTER 1**

**g0/0/0**



*ip access-list standard BRANCH-OFFICE-POLICY*

*permit 192.168.40.0 0.0.0.255*

*permit host 192.168.30.3*

*deny any*



*interface g0/0/0*

*ip access-group BRANCH-OFFICE-POLICY out*







<b>ROUTER 3</b>

<b>*g0/0/0*</b>



<i>access-list 1 remark PERMIT ALL TRAFFICS FROM **OFFICE 1**</i>

<i>access-list 1 permit 192.168.10.0 0.0.0.255 </i>

<i>access-list 1 permit 192.168.20.0 0.0.0.255 </i>

access-list 1 deny any



interface g0/0/0

ip access-group 1 out

