# Bruk av Webserver.

## Steg 1. Installer dependencies. 

- Gå inn i denne mappen:

    ````
    cd webserver
    ````

- Installer.

    ````
    npm install
    ````

- Installer også nodemon.

    ````
    npm install -g nodemon
    ````

## Steg 2. Importer dependecies. 

- Åpen filen [/server.js](server.js)

- Importere et bibliotek i JavaScript:

    ````javascript
    const express = require('express');
    ````

## Steg 3. Konsturere serveren:

- Konstruer og bestem en port prossen skal kjøre på.  

    ````javascript
    const server = express();

    const PORT = process.env.PORT || 5432;

    server.listen(PORT);
    ````

## Steg 4. Request 

- Ta i mot din første request: 

    ````javascript
    // Serveren tar i mot en 'get request' med ruten /hei. 
    server.get('/hei', (req, res) => {
        // Sender tilbake denne meldingen
        res.send("Heisan, hvordan går det?")
    });
    ````

## Steg 5. Start serveren.

- Bruk development serveren når du skal jobbe med den:

    ````
    npm run dev
    ````

- Kjøres på ekte:

    ````
    npm run start
    ````