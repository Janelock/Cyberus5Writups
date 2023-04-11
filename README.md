# Cyberus5Writups \

## who am i?
### first we checked the source code, we found a username and a password, we used them to login, we intercepted the request using burpsuite and sent it to the Repeater. On viewing the request we found a token, it looked like it was encoded and we recognized that it was encoded using base64. After decoding it, it's value was:login=Guest7, We tried changing it to login=admin, executed the request and the flag appeared.
### Flag: FLag{B@D_4uTh1Nt1C4Ti0n}


## bFlag
### We opened the file using wireshark, then searched in the packet details and we tried different words (e.g flag/fl4g..etc). We found an http request that included: /f14g/analyze_packet_for_fun and we deduced that it was the flag.
### Flag: analyze_packet_for_fun


## LOUDER
### We clicked on the provided link and downloaded the wav file, We then used a website that decodes an audio morse code and the output was:
### "T H E F L A G I S I A M S P E A K I N G L O U D E R T H A N B E F O R E"
### Flag: I AM SPEAKING LOUDER THAN BEFORE


## Hide Data
### We used a website that decodes caesar cipher, the output was:
"the flag is 2j68yfhqlz It is pretty easy to see the flag but can you see it i took nearly 1 minute to encode this with ROT13 good luck in solving that"
### Flag: 2j68yfhqlz


## Guess The Password
### We used a website that analyzes hashes, It recognized the hash as a sha1, we used another website that decodes sha1 and we found the flag.
### Flag: jrahyn+

