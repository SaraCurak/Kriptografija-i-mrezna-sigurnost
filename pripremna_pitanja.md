**PRIPREMNA PITANJA**

**LABORATORIJSKE VJEZBE 2**

1. What is the Address Resolution Protocol (ARP), and what is its role in a network?
    - ARP sluzi za pronalazenje MAC adrese odredisnog racunala na temelju njegove poznate IP adrese. Uloga je omoguciti da se uspostavi povezanost izmedu IP i fizicke (MAC adrese) u lokalnoj mrezi kako bi se paketi mogli isporuciti na ispravno odrediste.
  
2. What is a _Man-in-the-Middle (MitM)_ attack, and how does ARP spoofing enable it?
   - Man-in-the-middle je napad u kojem napadac ude u komunikacijski kanal s ciljem presretanja poruka izmedu dvije strane bez njihovog znanja.
   - Spoofing je pojam koji se koristi za opisivanje manipulacije mreznim podacima tako da se lazno predstavljaju kao da su poslani od strane neke druge osobe.
   - ARP spoofing - napadac se predstavi kao primatelj poruke odgovorom na ARP request, zatim te poruke proslijedi stvarnom primatelju. Napadac je "man in the middle", buduci da poruke uredno stizu do primatelja, strane ne znaju da ih se prisluskuje.

3. How does an attacker use ARP spoofing to intercept network traffic?
   - Napadac se predstavi kao primatelj poruke odgovorom na ARP request, zatim te poruke proslijedi stvarnom primatelju. Napadac je "man in the middle", buduci da poruke uredno stizu do primatelja, strane ne znaju da ih se prisluskuje.
  
4. How is the _cookie_ used to derive the encryption/decryption key?
   - Cookie se prosljeduje funkciji koja ce na temelju danog stringa derivirati enkripcijski/dekripcijski kljuc.

5. What REST API request do you need to send to the _crypto oracle_ the secret cookie?
   - GET request
  
6. How do you obtain the authentication token?
   - Man-in-the-middle napadom, na komunikaciju racunala arp_client i crypto oracle servera. Crypto oracle ce poslati autentifikacijski token.
   
7. How do you use the authentication token to obtain the cookie?
   -Nakon presretanja autentifikacijskog tokena, mozemo se autentificirati i poslati GET request na /arp/cookie.

8. What encryption mode is used to encrypt the challenge in this lab?
   - CBC

9. What tool can you use to capture network traffic on a local network interface?
    - tcpdump

