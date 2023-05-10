# Laboratorio Angular per il corso di Sviluppo di Servizi Web
Il laboratorio consiste in un container Docker con:
- un server `NoVNC` che offre un desktop Ubuntu
- l'installazione di `Node.js` completa del tool `npm`
- l'installazione del framework Angular 2+
- una applicazione di editing orientata allo sviluppo (`geany`)

Per realizzare il laboratorio, clonare questo repository.

Per mandare in esecuzione il Docker, dipendentemente dal supporto Docker installato:
- per Docker Desktop digitare il comando `docker compose up`
- per Docker Engine digitare il comando `docker-compose up`
(la differenza tra i due è il trattino)

Nella directory `labssw` che verrà così creata trovate:
- una directory `shared`. Serve a condividere file tra la macchina host e il Docker in esecuzione. Nel Docker, la directory corrispondente si troverà nella directory `Desktop`
- una directory `ssh-keys`. Contiene le chiavi ssh per accedere a server esterni, ad esempio github. Le chiavi vengono costruite nella macchina host. Nel Docker la directory corrispondente si trova nella home dell'utente `user`. Per maggiore sicurezza le chiavi non sono conservate nella immagine ma nel filesystem della macchinahost.

Il desktop è accessibile tramite il browser della macchina host alla URL [http://localhost:6080](http://localhost:6080)
