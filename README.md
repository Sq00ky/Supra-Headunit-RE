### Overview
This repository contains resources related to reverse engineering the Toyota Supra Headunit firmware.
### Remounting the Filesystem as RW
mount -o remount rw /net/hu-omap/fs/sdaX
credit to @a90.faraz
### SSH Connection
Pre-Req: Ethernet -> ODB2 cable (Also known as eNet).
1. Message the guys @ FlashXCode on Whatsapp, be sure to ask them to enable SSH, include your VIN & iStep version number (can be found under Navigation > Settings > Position and software version > software version) - https://www.flashxcode.com/product/feature-installer-code/
2. Paypal them 25 Euros as Friends and Family
3. Download FeatureInstaller
4. Run FeatureInstaller, wait for it to scan then select "Identify" when you've found the car
5. Input the code provided by FlashXCode
6. Wait for it to finish

Afterwards, you can ssh into:
ssh root@169.254.199.99
ts&SK412
### Misc User Account Credentials
**Plaintext**
```
root:ts&SK412
browser:browser
hmi:hmi
scp:scp
sys:sys
nav:nav
mm:mm
pd:pd
```

**Hashes**
```
browser:6sT7U.GRTdFHc:15492:0:0
conn:q5WlBiLI3VkBM:15492:0:0
hmi:w2mp4wK0yla6I:15492:0:0
mm:1gcF8pvCWAjb.:15492:0:0
nav:3jgsx4NqHnuiE:15492:0:0
pd:4lt4bcpTMrsQQ:15492:0:0
root:7x/CyxnY..rkQ:15492:0:0
scp:b9zWTRVRNJ4xg:15492:0:0
shell:r31lc4zUATwYg:15492:0:0
sys:0fRl8SwCuDmmI:15492:0:0
```
**SSH Key**
```
-----BEGIN RSA PRIVATE KEY-----
MIIEoAIBAAKCAQEAtuXhwEjQjFuZhKdo1YH1QRulRzzyoUZIxdgz//q8NA4Z+jws
H71DGsDkWDklIHP2g505VuDmzjz3No6iFpdfHArInzaz7Wh67OtWvg7yEgxhdDNu
gaup/q0Yjaadx+PSfVF3JE6cAMH/87xOF/HUU0sMYPEW36YV18C96mYRCDwI1OgM
93ygHHd7ZmkC5LBgjLQpgi8shNqCBLKYLML82w0B9h7ULEZMolckO2CY8SCtvURV
ckLmgIg9a4F7laxywFy7kLuoY17erOB/4b6xbkSO46H2wKGr/SKLnSBnvUBY8FKl
jDgLCRr42fwHBRQk3FOBpiMPG/RiMWpEbZjJvwIBIwKCAQBjSZfOyHE2QFqnGQ0G
MJsUtzx3IRX/xxGP+QZJIbaf6mXfnQICmfE6aLZ5CRQnj2iQly3BcsZv9TW+h/GX
PDrx9zm1hBiIMWdNadAAxkjlOevCvNWW2YgrKsQvo5d7I+dLWBwbBhosTA6aQaa8
ipfVceIl/zhNhgvbheNwnc67Ut5x4bbozVwOrZhXnqyLgDUlnPSexU2LrP0okNH8
v49fTtsgf6i5qIfcFA5lwGa98kZLa4CC1ZaPbofa4GZtSaPU9lsgAb0pi3slYxYP
ciMH9/GFGex6zYTQvAN+9IqS5M2fMvVk7+DwIfD+1nT/fFPBHfPJTIEYZP6iQ6th
TL77AoGBAOw4rqZzVg2G8Bx6ZAGtIoMudqRsUF2QOKO9tN7IuNvkipnp9DPV/Rvr
FOb8I2cJawl6zLzl1dcBcgJxRLyVx2N07D5xXxmtotOub6L02nN3lHMf0nSlPGOt
CZ7M3vX+x7RjB2wzCbsPvJBVs9a8WoZ34unbTdUlQoeu4ybW8BDpAoGBAMY2O0t4
/R7mR5ciMY158ojwiC5CPXYAzv51hykZL/3ooE2n4SYotGxXvvpN6D6/s/pZOE2A
d9G6PSXFXAJRhdQGgkEM0p4K44Z2M5lXLO/1e5TBJn2k+Cs7YESwfvk2nUS43+EY
geeCY0DJypwhQGJsfMk9EmcamX6174OSlJxnAoGAUP19tWlfVRhSUugiSbe0D7go
rWb2+4HniJjQTGITfpd/+kGVjh17Wgd04XsE0t6oWwWIBkAsDzOyD3dKxFCcIhl1
kcB4YJNNxOtZebMJEaVXd+2nPe+Ca1FFIIDBeOmjjk3WqMEKpokNc1CVbjHzJsoE
p/NrJIHNqtzgKpLV9ysCgYBJnx1WjAY+rU3Ka8lDLUt0sRyjd7BtqIdl0+G+ztdP
rizppMFXUPKOpD+ezHrVemdrnXtP/IRGlaGu8YiTJZgbjWOUgRsHgGMjUHmQufq/
hxCk90jPlQu4SUEDkgNGn0G6cI2rYN/LBItD8y3/ehCZlgJ2oae/5U70jLgMTGMV
hQKBgC138Od6PZT2ZlTl8seRuNXqcv9unwYvDR5yZCg2eJNIq+o+wQLcJiDCFCre
UBjlshupt5emCPsp3Cp2zPn9zowYpvzqnnv7J6s1CzGJQME96o2sBq4rc+tSYKXI
+DNqXJjzZULDRdFrdpUpeIKLDq0WLIJeihiCdr9vQnexL7W7
-----END RSA PRIVATE KEY-----
```

```
-----BEGIN DSA PRIVATE KEY-----
MIIBuwIBAAKBgQDpJJMKrXIuAwb2rDTYzrWaWcRk8YNs3FionsYKjYVU1ssoQn59
wcPSt8EyQBI7+Z+uAsPA1M6YjZjyT8Yqps/8h4bzrUTM5ag3tukXjdq3zz/3p80r
CHaEsE/DS1F/KG922m3WY2Dpn+3/5XdQrs8hw6OBlrfx7RUOBcyJiaPT6wIVAJNS
rZ+ZAaTnVlZ+BhkUwfu/zuUTAoGBALgXU3JDEW1+ZlbnPtKH5/RVUza/Sl2mn1Sz
NXq86dzwuwEBSx9tqfPALPlyNJEfxJYUOd+8/skxMOh7Qm5FdGBUNfu6cHiT/Ty6
aSDJ/in3qq8/5yGe2it+YgCwMf5squr+17SxC3fEldNL7sHPElVDFwkN3W3bwZtP
/imyzwAuAoGAI3gCp7avWAdaOcGijOzu85w/WK3Yx1BZGkoGwYR6LPRlUJYbVnRm
nMOYbSDLkvvQXwWlgU6Hx3W+TLfkqqpfodGAmtz3Ots1d8KqPudzADxhz5ku2dJd
s8draRo4qqaVD8VLgM8tXQMCevHj3NFLrETtxD0G1vJT96KatHEH2jYCFBWvuTB5
ZX5vWp+Tj/da+KL6OrYv
-----END DSA PRIVATE KEY-----
```

### Ownership
All rights belong to Toyota (Toyota Motor Corporation) , BMW (Bayerische Motoren Werke AG), and Harman Kardon (Harman International)
