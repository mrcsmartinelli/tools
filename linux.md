# Creare / Eliminare utente

sudo adduser nome_nuovo_utente
sudo adduser nome_nuovo_utente sudo
sudo deluser old_utente
sudo rm -rf /home/old_utente

# Aggiornare

1. **sudo apt-get clean** - Ripulisce la cache locale dei pacchetti
2. **sudo apt-get update** - Scarica la lista aggiornata dei pacchetti e delle nuove versioni disponibili nei repository. Questo comando si limita a recuperare informazioni, ma, in concreto, non installa nulla
3. **sudo apt-get dist-upgrade -y** - E' il comando principale, poiché scarica ed installa le ultime versioni dei pacchetti, delle dipendenze ed, eventualmente, il kernel più recente. In ogni caso, non esegue mai l’avanzamento di versione
4. **sudo do-release-upgrade** - Esegue l’avanzamento di versione, passando alla release di Ubuntu successiva
5. **sudo apt-get autoremove -y** - Rimuove tutti i pacchetti obsoleti e non più necessari

Fonte: https://www.bartolomeoalberico.it/aggiornare-ubuntu-da-terminale
