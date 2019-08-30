

## 1) Monitoring HTTP Headers 1

### Observe and explain each of the values monitored (use view source to see the plain messages).

Jeg ztrl+shft+j og går til network taben. Her ser jeg 2 requests.
Ser index filen med hello world! 
og Favicon som er tomcats logoet som icon.



Efter jeg ændre til index1 og pejer til index1.html ser jeg det samme.

## 2) Monitoring HTTP Headers 2

### explain the purpose of the connection header.

Holder styr på hvorledes forbindelsen skal forblive åben efter transaktionen er færdig. Med fx. keep-alive er forbindelse persistent og så kan der lave felere request til samme server.


## 3) Monitoring HTTP Headers 3  (Response-codes 3xx)

### forklar de to requests:

Først ser jeg redirect responset.
Den har status kode 302, som er et redirect.
Derefter kommer resourcen.

Når jeg refresher er der ikke noget redirect svar, da jeg er på den rigtige resource nu.

## 4) Status Codes
### 4a) Status Codes (5xx)

Fordi jeg har ramt en singularity issue ved at dividere med 0, kaster serveren en kode 500 fordi servletten har kastet en exception.


### 4b) Status Codes (4xx)
gode gamle kode 404, den resource existere ikke, og derfor kommer der en 404 tilbage.

### 4c) Status Codes - Ranges


2xx er succes coder for alle succefulde requests

3xx er redirects, dvs at de pejer til det man leder efter

4xx er client side errors, så man har bedt om noget forkert.

5xx er server errors. Dem skal man jo helst undgå.

eller:

1xx: hold on

2xx: here you go

3xx: go away

4xx: you f$*%ed up

5xx: I f$*%ed up

## 5)
Done did the thing.

## 6) Get/Post-parameters

### Observe what happens in your browser's address field.

Det hele bliver sendt som url og man kan se det i search baren.

inkl hidden værdien og action. som query string parameters

### Use post method: Write down your observations

Hidden værdien bliver ikk længere passet som en del af URL, men kan ses under form data.


## Session og Cookies:

### Session:

Forskellen på session og cookies er hvor de ligger henne.

Sessionen er kun på tomcat siden, og bruges til at holde styr på vigtig information om det nuværende besøg. Et almindeligt exemple er at holde brugeren login her, eller alle de ting vi regner med brugeren arbejder med.

Som standard er tomcat sat til at udløbe sessionen efter 30 min.

### Cookies:

Cookies bruges som en lokal ting på din computer til at holde styr på vigtig information for dig, det kan være logins information, Inkøbs kurv status etc. Ting der er vigtig for brugeren over flere besøg, vor session kun er ting der er vigtige for dette besøg.