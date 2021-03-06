# SOS Circolari

## Elenco features
TODO

## Requisiti
- [Docker](https://docs.docker.com/install/)
- [docker-compose](https://docs.docker.com/compose/install/)
- [npm](https://www.npmjs.com/get-npm)

## Struttura repository
- `logs` contiene gli access ed error logs
- `src` contiene il codice del componente SOS Circolari
- `.env.sample` è un file di esempio che contiene la struttura del richiesta per il file `.env`

## Struttura componente
- `admin` contiene le parti del componente per l'admin panel
- `site` contiene le parti del componente per il frontend
- `media` contiene i files statici, ovvero `.js`, `.css` e immagini
- `script.php` permette di inserire alcuni scripts per gestire particolari lifecycles del componente
- `sos_circolari.xml` è il file manifest 

## File index.html
Il file index.html presente in ogni cartella del progetto serve per prevenire la navigazione diretta delle directory 
da indirizzo web.
[Più informazioni](https://stackoverflow.com/questions/29224471/joomla-index-html-file)

## Istruzioni per lo sviluppo
1. Installare i requisiti
2. Avviare il daemon di Docker
3. Eseguire `cp .env.sample .env` (ed eventualmente modificare le variabili d'ambiente)
4. Eseguire `npm start`
5. Installa il componente da console web andando all'indirizzo 
`http://localhost/administrator/index.php?option=com_installer` e cliccando `Install from folder/Check and install`

Le modifiche fatte ai vari files dentro alla cartella `src` 
saranno subito visibili in seguito al primo refresh della pagina.
