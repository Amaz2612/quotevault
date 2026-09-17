# QuoteVault

Webapplicatie om quotes te ontdekken, doorzoeken en bewaren. Gebouwd voor het project "JS OOP en MVC" met vanilla JavaScript, zonder frameworks.

## Functies
- Quote van vandaag (vast per dag, opgeslagen in LocalStorage)
- Willekeurige quote ophalen via de API
- Zoeken op woord of auteur, met paginering
- Favorieten bewaren met een persoonlijke notitie (LocalStorage)
- Reservekopie van quotes als de API niet bereikbaar is

## Starten
ES-modules werken niet via `file://`. Start daarom een lokale server:
- **VS Code**: installeer de extensie *Live Server*, klik rechts op `index.html` en kies *Open with Live Server*.
- **Of** in deze map: `npx serve` of `python -m http.server`, en open de getoonde URL.

## API
[DummyJSON Quotes](https://dummyjson.com/docs/quotes), geen API-key nodig.
- `GET /quotes?limit=0` alle quotes
- `GET /quotes/random` een willekeurige quote

## Structuur (MVC)
- `js/models/` data, API, LocalStorage (geen DOM-code)
- `js/views/` HTML opbouwen en gebruikersacties doorgeven
- `js/controllers/` koppelt model en views
- `js/app.js` maakt alle objecten aan en start de app
- `docs/` projectwijzer, UML-diagrammen, demo-voorbereiding
