# Cyberus5Writups
## who am i?
#### first we checked the source code, we found a username and a password, we used them to login and we intercepted the request using burpsuite and sent it to the Repeater. On viewing the request we found a token, it looked like it was encrypted and we recognized that it was encoded using base64. After decoding it, it's value was:login=Guest7, We tried changing it to login=admin, executed the request and the flag appeared.
#### flag:FLag{B@D_4uTh1Nt1C4Ti0n}
