# Trading Algoritme. 

## Steg 1. 
- For å komme i gang med algoritmisk trading må du først opprette en konto på [alpaca markets](https://alpaca.markets/).

- Her finner du også din API-key og secret-key på _Paper Overview_ under _Your API-keys_. 

- Mer dokumentasjon om API'en finner du [her](https://alpaca.markets/docs/trading/). 

## Steg 2. 
Installer python pakken for alpaca sin api:

- Føst sjekk at du har pip3 installert:

    Åpen terminal på mac, eller Powershell på windows og skriv inn: 
    ````
    pip3 --version
    ````

    Da skal noe lignende komme frem:
    ````
    pip 22.2.2 from C:\Program Files\WindowsApps\PythonSoftwareFoundation.Python.3.10_3.10.2032.0_x64__qbz5n2kfra8p0\lib\site-packages\pip (python 3.10)
    ````
    Kommer det en feilmelding kan det være lurt å innstalere python på nytt. 

- Installer så pakken:
    ````
    pip3 install aplca-trade-api. 
    ````

## Steg 3. 

- Importer pakken i python programmet:

    ````python
    import alpaca_trade_api as tradeapi
    ````

- Definner variabler for _end point_, _api key_, og _secret key_

    ````python
    END_POINT = "https://paper-api.alpaca.markets"

    API_KEY = "<Din API-key>"

    SECRET_KEY = "<Din secret key>"
    ````

- Lag så en klasse hvor du deffinerer følgende funksjoner:

    ````python
    class myTradingBot:
        def __init__(self) -> None:
            self.bot = tradeapi.REST(API_KEY, SECRET_KEY, END_POINT, api_version="v2")

        def buy(self):
            # Din kode her. 

        def sell(self):
            # Din kode her. 
    ````

## Steg 4. 
Slå deg løs!! :grinning:


![Go wild](https://c.tenor.com/huuQ4PxKMTYAAAAC/madagascar-alex-the-lion.gif)

---

# For å bruke _`clap_and_trade.py`_

## Steg 1. 

- Installer følgende pakker:

    ````
    pip3 install alpaca-trade-api numpy sounddevice
    ````

    Dersom det ikke går i _one go_ ta en etter en:

    > alpaca-trade-api

    > numpy

    > sounddevice

## Steg 2. 

- Pass på at du har en fungerende microfon på PC/Mac'en din, bruk av headset / airpods / etc anbefales. 

- Endre i så tilfelle input mikrofonen din i innstillinger. 

## Steg 3. 

- Pass på at du er i rett mappe:

    ````
    cd algo
    ````

## Steg 4. 

- Kjør programmet!

    ````
    python3 clap_and_trade.py
    ````

- Først vil den stå å jobbe litt

- Derretter etter at følgende blir printet:

    ````
    Starting....
    ````
    Er det bare å klappe i vei! :clap: :clap: