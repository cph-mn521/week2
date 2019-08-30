

### 27:



## What is your public IP address right now, and how did you find it?

til public bruger jeg* [ip4.me](http://ip4.me/) 

## What is your private IP address right now (do this both at home and in school), and who/what gave you that address?


Jeg finder min IP ved at åbne powershell og skrive ipconfig.
   IPv4 Address. . . . . . . . . . . : 10.50.131.77


### What is special bout these ranges:

## 10.0.0.0 – 10.255.255.255 
Class A – 24 bit blok

## 172.16.0.0 – 172.31.255.255 
Class B – 20 bit blok.

## 192.168.0.0 – 192.16 8.255.255
Class C – 16 bit blok.


## What’s special about this ip-address: 127.0.0.1?
Loopback addresse 

returnerer alt til samme adresse, til test af tcp/ip netværk. (localhost)

### What kind of service would you expect to find on a server using these ports: 

## 22

Denne er til SSH remote Login Protocol.

## 23
Telnet - bruges til remote accesing af andre computere på netværket.

## 25
SMTP - Simple mail transfer protocol

Den til mail.

## 53
DNS

## 80
HTTP

## 443
HTTPS


### What is the IP address of studypoints.dk and how did you find it?
165.227.137.75 – powershell: ping studypoints.dk
157.230.21.145 – powershell: ping studypoints.info

## If you write https://studypoints.dk in your browser, how did “it” figure out that it should go to the IP address you discovered above?
DNS. det er det der er skabt til, omdanner ip adresser til domain navne. Står for Domain Name System.

## Explain shortly the purpose of an ip-address and a port-number and why we need both
Ip adresser er min identitet.
Porte er identiteter på services på min computer.

## What is your (nearest) DNS server,?
Min router.

## What is (conceptually) the DNS system and the purpose with a DNS Server?
Opslags værk med navne og deres tilhørende adresser.

## What is your current Gateway, and how did you find it?
Default gateway: 
Default Gateway . . . . . . . . . : 192.168.0.1   --- min routers addresse.
powershell - ipconfig /all


## What is the address of your current DHCP-Server, and how did you find it?
Samme som ovenstående.

## Explain (conceptually) about the TCP/IP-protocol stack

Kommer fra OSI modellen, der er en 7 lags standardiseret måde at forbinde over netværk.
TCP/IP er en mere anvendt samling protokoller 4 lag.
-kabler
-ethernet
-IP
-TCP/UDP, multiplexing par.

## Explain about the HTTP Protocol (the following exercises will go much deeper into this protocol)

Hyper Text Transfer Protocol - den standardiserede måde vi er blevet enige om at sende data på nettet med. Fungere som bindelede mellem client og server.

Bygget op omkring et request/response med en Body(Indhold) og en Header(Metadata).

## Explain (conceptually) how HTTP and TCP/IP are connected (what can HTTP do, and where does it fit into TCP/IP)

HTTP er et set regler, som existere i applications laget af TCP/IP. Hvilket betyder at det definere reglerne for udveksling af request/responses.

server_name matheradical.dk www.matheradical.dk;
