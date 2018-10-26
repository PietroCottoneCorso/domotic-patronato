## Cosa fa questo programma
Programma domotico per uso domestico che permette l'accensione di luci da remoto
il progetto utilizza un Raspberry pi 3b e una scheda relè

![IMMAGINE](https://image.ibb.co/eoFCVq/openhab-screen.png)

## Software
software basato su **Openhubian** e **MQTT**. 
Le luci si attivano tramite Cloud su OpenHub.
# Installazione
1. Installare Openhabian tramite [GUIDA UFFICIALE](https://www.openhab.org/docs/installation/openhabian.html#quick-start)
1. Prima del primo avvio creare un file `ssh` vuoto nella root della SD togliendo qualsiasi tipo di estensione
1. Trovare l'ip del raspberry connesso alla rete e utilizzate un client SSH (Putty) per connettersi. Per connettersi inserire come user e Password `openhabian`
1. Aggiornare sistema con:   
    ``` 
    sudo apt update  
    sudo apt upgrade  
    ```
1. Nella cartella `/etc/openhab2/items` creare il file `[user].items` e definire i pin di collegamento con il relè
1. Entrare nella cartella `/etc/openhab2/rules` e creare il `[user].rules` e definire le regole degli interruttori

## Hardware
BOM:
* Raspberry Pi 3B+
* Modulo Relè Optoisolato, con il numero di canali necessari
* Jumper Dopont
* Led
* Pulsante

## =D
