# Browser Technologies
// Robuuste, toegankelijke websites leren bouwen …

Feedback:
## Tabs
1. Instead of using `#` on `<a>` tags, link them to sections
2. The tabs are unneeded if javascript is does not work.

**Fix**
1. Applied `id`'s to the sections and linked to them explicitly in the tab instead of using `#`
2. If `getElementByClassName` is not supported the tabs will be removed

- The nav is by default hidden now and will be shown if JS is enabled and `getElementByClassName` is supported.

Also created a function to check on eventlisteners support.

## Image Picker 2
1. The `<img>` placeholder is clutter if `FileReader` is not supported 

**Fix**
1. Load in the `<img>` placeholder if the `FileReader` is supported 



**[Tabs](https://kyunwang.github.io/browser-technologies/opdracht2/tabs/)**

**[Image picker] - does not use `<input>`(https://kyunwang.github.io/browser-technologies/opdracht2/image-picker/)**

**[Image picker 2](https://kyunwang.github.io/browser-technologies/opdracht2/image-picker/image-picker2)**
# Opdracht 2 - 1, 2, 3 Feature Detectie
// Wat laat je zien als een browser of gebruiker 'enhancement' niet kan tonen of zien? Hoe doe je Feature Detection en wat doe je als een techniek niet werkt?

Werk 2 componenten uit in een demo. Je onderzoekt hoe je verschillende features door verschillende browsers worden ondersteund en hoe je voor goede fallback kan zorgen. Gebruik html5test.com, css3test.com en kangax.github.io/compat-table/es6/

Per component: Schets hoe het component moet gaan werken en hoe het eruit komt te zien. Verzamel uitleg en artikelen. Bouw een (kleine) progressive enhanced demo (zonder extra tools, gewoon in 1 HTML file inclusief CSS en Javascript, zo simpel mogelijk). Test het component op verschillende browsers en het Device Lab. Polyfills en NPM is niet toegestaan.
Post je 2 demo’s op GitHub met uitleg in een README file. Wat is het component? Voeg je schets toe. Welke browsers/devices ondersteunen deze wel/niet? Hoe zorg je dat de Core Functionaliteit overal werkt?
Beoordelingscriteria
2 componenten zijn onderzocht en er is een demo gemaakt.
De code staat in een repository op GitHub.
Een Readme is toegevoegd met, per component:
Een beschrijving van het component.
Een schets van de functionaliteit.
Bronnen van uitleg en gebruikte artikelen.
Welke browsers/devices ondersteunen deze wel/niet.
Een beschrijving hoe je ervoor hebt gezorgd dat de Core Functionalitiet het overal doet.
Componenten
Kies minimaal twee componenten. Één van de Romeinse en één van de Arabische serie.

i. FAQ lijst, een vragen lijst over de verschillende minorvakken ii. Tabbladen, de 5 studenten met de meeste kudo’s iii. Accordeon, de drie favoriete docenten met meer informatie iv. Responsive menu, dat een hamburger wordt op een klein scherm v. … egen idee? Kom maar overleggen

Carrousel van een aantal aankondigingen (met tekst en links in de tekst)
Link + overlay/modal-window met algemene voorwaarden of extra specs
Image picker + preview, voor als je een profiel foto wil uploaden naar je favoriete sociale netwerk
Routebeschrijving van huis naarKSH , die stap voor stap op een kaart laat zien waar je heen moet
… eigen idee? Even overleggen