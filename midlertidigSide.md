# Vi trenger en midlertidig side til domene!

## Krav:

### Bruk av teknologi:

- Du skal kun bruke vanlig HTML, CSS og JavaScript for denne siden. 

- Lag en ny mappe på din PC og sett i gang! :)

### Logo

- Det første som vises er logoen vår.

- Bruk bildene som ligger [her](https://github.com/nathsten/fintech-krasjkurs/tree/main/docs/images)

### "Comming soon"

- Det skal stå noe slikt at nettsiden kommer snart.

### Mulighet for å vise til sponsorer og sammarbeidspartnere

- Gjør det enkelt å legge til sammarbeidspartnere som Enigma og eventuelle logoer til sponsorer nederst på siden. 

### Design

- Bruk et kult design, bruk fargene som ligger i [pdf-filen](https://github.com/nathsten/fintech-krasjkurs/blob/main/docs/images/GrafiskProfil01.pdf) som omhandler logoene


- Bruk noen kule fonter, eks: (pleier å være bankers)

````css

.minOverskrift{
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

````

- Legg til noen kule animasjoner e.l, få de sirklene til å bevege seg i bakrgunnen e.l

- Animasjon lages slik:

````css
.minAnimerteDiv{
    width: 50px;
    height: 50px;
    background-color: blue;
    animation: minAnimasjon 2000ms infinite forwards;
}

@keyframes minAnimasjon{
    0% {left: 20rem;}
    50% {left: 10rem;}
    100% {left: 20rem;}
}
````