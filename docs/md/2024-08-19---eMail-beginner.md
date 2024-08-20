#Link https://www.youtube.com/watch?v=ACTC7N38kYo

#Link 

____________

```bash
	umask
```
.

```bash
	0022 #Sicherstellen , dass 0022 steht
```
.
```bash
	cd /opt/
```
.
```bash
	sudo apt install git
```
.
```bash
	git clone https://github.com/mailcow-dockerized
```
.
```bash
	cd mailcow-dockerized
```
.
```bash
	./generate_config.sh
```
.

#eMail-mailcow 
 - [[2024-08-19---eMail-mailcow.config]]

```bash
	vim mailcow.conf
```
.
```css
	mail.ydh.solutions  # Full Qualified Domain Name [FQDN]
```
.
- lädt aus dem yml - File alle aktuellen Packages
```bash
	docker-compose pull
```
.
- wir installieren die Packages
```bash
	docker-compose up -d
```
. 
- wir lassen uns alle docker anzeigen
```bash
	docker ps -a
```
.
- wir loggen uns bei mailcow ein (mail.ydh.solutions)
- lassen uns den "netfilter" anzeigen mit: 

```css root@mail:/opt/mailcow-dockerized#
	docker ps -a | grep netfilter
```
.
- wir installieren den Fail2ban

```css
	sudo apt install fail2ban
```
.
- wir schauen uns den Status an
```css
	fail2ban-client status sshd
```