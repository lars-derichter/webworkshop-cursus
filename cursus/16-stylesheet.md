# Stylesheet

## 🧪 Weergeenstijl

Was je ook zo verdrietig of gefrustreerd toen je cv.html in je browser bekeek? Het leek wel of de stijlen waaraan je zo hard gewerkt had in index.html niet bestond. Tenzij je dacht dat je een slimmerik was en je ze gewoon vanuit het head van index.html naar dat van cv.html gekopieerd hebt. Voor twee pagina’s lukt dat nog, maar stel je eens voor dat je de sitebeheerder bent van de Thomas More website en plots beslissen ze dat het Thomas-More-rood één tintje donkerder moet overal. Je kan moeilijk alle 3000 pagina’s overlopen en die één voor één aanpassen. Er moet een betere manier zijn!

Uiteraard is die er ook: je kan alle stijlen (of een deel van de stijlen) van je website samen zetten in één apart bestand en vanuit elk html-bestand daar naar linken. Dat is al een stuk minder werk en zo wordt het veel makkelijker om je stijlen te beheren.

Daarvoor ga je als volgt tewerk:

 1. Je maakt in dezelfde map als je index.html een nieuw bestand met de bestandsextensie .css (bijv. styles.css).
 2. Je knipt de hele inhoud van je style-tags (maar zonder de style-tag zelf) en plakt die in het css-bestand.
 3. Je verwijdert de style-tags en waar die stonden (in je head) zet je de volgende tag:

```html
<link rel="stylesheet" href="styles.css" />
```

Je css-bestand ziet er ongeveer zo uit:

```css
html {
  font-family: "Source Sans Pro", Arial, "Helvetica Neue", Helvetica, sans-serif;
}
h1 {
  font-size: 24px;
  line-height: 26px;
  color: #f04c25;
  font-weight: 900;
}
```


Als je dat in het head-element van al je html bestanden doet, krijgen ze allemaal dezelfde uniforme opmaak en dat is wat we hier willen.

 <table style="width: 100%; border-collapse: collapse; border-style: none;" border="1">
    <tbody>
        <tr>
            <td style="width: 8%; border-color: #009cab; background-color: #009cab; text-align: center; vertical-align: middle;"><span style="font-size: 36pt;">ℹ️</span></td>
            <td style="border-style: solid; border-color: #009cab; text-align: left; vertical-align: middle;">
                <ul>
                    <li>het link-element is voor links die de browser nodig heeft &harr;︎ het a-element gebruik je voor links die de gebruiker kan volgen.</li>
                    <li>het rel-attribuut geeft aan wat voor type link het is; hier is het een stylesheet dat de browser kan gebruiken om de inhoud op te maken</li>
                    <li>het href-attribuut is de url waarnaar gelinkt wordt: hier het styles.css bestand dat zich in dezelfde map bevindt als het html-bestand waarin deze link staat</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>

## Stylesheet

Zo een apart css-bestand met stijlregels in noemen we een stylesheet.
