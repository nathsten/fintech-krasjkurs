# Spesifikasjonskrav 

## Meny

> En meny som linker til alle fanene våre (om oss, blog, etc)

> Må være responsiv (passer for både PC og mobil). Så lenge ferdige Docusaurus rammeværk er i bruk er det tatt hånd om. 

## Landingsside. 

> Bilde og kort tekst om fintech enigma. (Typ. slagord e.l.)

> Graf av noe slag som viser proteføljen vår (finn på noe) sammen med noe kort forklarende tekst. 

### Tips:

* > Sjekk ut [chart.js](https://react-chartjs-2.js.org/).

* > Bruk ellers et bilde

<br>

> Graf som viser til en tradingalgorime sammen med noe kort forklarende tekst.

> Skal også være en link som viser til algorime proteføljen* vår (Hvor vi gjerne har flere). 

> Bruk kreativiteten fritt og implimenter det du føler er viktig å ha med på en landingsside!

## Design. 

> Bruk CSS, gjerne ferdiglaget som dere finner på nett til å gjøre ting så fint som mulig. **NB** Pass på at dere ikke bruker _statiske_** designmetoder. 

## Hvor finner du filene for landingssiden?

- Filen for hjemmesiden ligger under [src/pages/index.js](./src/pages/index.js)

- Filen som genererer `HomepageFeatures` ligger  i [src/components/HomepageFeatures/index.js](./src/components/HomepageFeatures/index.js)

- Bildene ligger i [static/img](./static/img/)

Prøv å lek dere i disse overnevnte filene for å manipulere hjemmesiden til slik dere ønsker at den skal se ut. Det er bare å slå seg løs å prøve seg frem!

<br>

### Fotnoter


\*Lag en side under ````./docs```` som f.eks. heter ````algoritmeportefølje.mdx```` hvor dere kort finner på et par algoritmer og skriver noe oppfunnet tekst. Link så denne siden til der hvor grafen til en av algoritmene vises på landingssiden. 

\*\*Statiske designmetoder er feks: 
````CSS
.myclass{
    width: 120px;
    height: 80px;
    position: relative;
    left: 30px;
}
````
Her er bredde, høyde og posisjon bestemt av pixler som vil se veldig dårlig ut når en går fra en stor skjerm til en liten skjerm. 

Sjekk ut tips for responsiv design:

* [Intro](https://www.w3schools.com/css/css_rwd_intro.asp)

* [Mer dybde](https://www.toptal.com/front-end/dynamic-css-with-custom-properties)

* [Tailwind CSS](https://tailwindcss.com/) er en enklere måte å skrive responsiv HTML uten mye kode (krever litt forkunnskaper).

* > [Innstallerings guide](https://dev.to/sajclarke_62/using-tailwindcss-v3-in-docusaurus-in-5-steps-5c26), 
<br>**NB:** Hopp over _Step One_ dersom du jobber i dette prosjektet. 
<br>**MERK:** i guiden brker de: ````yarn add tailwindcss postcss autoprefixer````. Erstatt det med følgende:

    ````
    npm install -D tailwindcss
    ````

    ````
    npm install tailwindcss postcss autoprefixer
    ````

* >Erstatt også ````yarn start```` med:

    ````
    npm run start
    ````

* > For å _[kompilere](https://tailwindcss.com/docs/installation)_ input filen bruk følgende utgangspunkt:

    ````
    npx tailwindcss -i ./<mappe med input.css>/input.css -o ./<outputmappe>/output.css --watch
    ````