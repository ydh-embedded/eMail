
#LINK https://www.youtube.com/watch?v=6X6GrJhG_q4

__________

```css 
	SKIP_LETS_ENCRYPT=n  
```
.
```css
	SKIP_CLAMP=n
```
.
```css 
	SKIP_SOGO=n  
```
.

#Solar Solar kann die Mails mit Indizes versehen um die Suche zu optimieren

```css
	SKIP_SOLR=n
```
.

#Watchdog 
- Bei SPAM Attacken kann hier eine E-Mail eingetragen werden damit man über den Angriff informiert wird
```
	WATCHDOG_NOTIFY_EMAIL=ydh.monitooring@yahoo.com
```
.
```css
	WATCHDOG_NOTIFY_BAN=y
```
.
```css
	WATCHDOG_SUBJECT="Mailcow: "
```
.
 #Docker-Compose-YAML 
 - wenn man die IP in der config ändert muss auch die YAML - Datei von Docker - Compose angepasst werden (wird in 1ter Instance nicht getestet)
```css
	IPV4_NETWORK=172.21.22
```
.
 #Certificate 
 - eMail Benachrichtigung sobalt LetsEncrypt Certificate ablaufen sollten
```css
	ACME_CONTACT=acme@ydh.solutions
```