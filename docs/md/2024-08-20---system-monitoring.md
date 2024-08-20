#LINK https://www.youtube.com/@RaspberryPiCloud


______________
# Linux
## Benchmark / Testlauf

### CPU

- wir testen Events
```css
	sysbench cpu run
```
.
### RAM

- Transfer Rate beachten :-) MiB/sec
```css
	sysbench memory run
```
.
### RAID / M2

- Sequenzielle(synchron) Schreib-Geschwindigkeit
```css
	sysbench fileio prepare
```
.
```css
	sysbench fileio run --file-test-mode=seqwr 
```
.
