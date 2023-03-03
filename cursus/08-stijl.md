## Geen stijl

Op dit moment ziet je pagina er nog heel saai uit, ze heeft gewoon geen shtijl.

We zouden (voorlopig) graag hebben dat onze pagina een beetje aangepast is aan de Thomas More huisstijl. Zoals dit dus:

Jullie zullen nu proberen om je pagina’s hetzelfde uitzicht te geven.

## Regels om CSS-regels te maken

 - Onderaan in je head-element, voeg je een style-element <style></style> toe. Daarbinnen ga je de CSS stijlregels zetten.(⚠️ Dit is niet de voorkeursmethode om stijlinformatie toe te voegen aan een HTML-document, maar wel handig als je iets wil uitproberen.)
 - Een CSS-regelset begint met een *selector.* Daarmee kies je voor welke elementen de regels gelden. De eenvoudigste selector is de naam van het element bijv. h1.
 - De inhoud van de CSS-regelset staat tussen accolades { en }.
 - Elke CSS-regel begint met de naam van een eigenschap (*property*), gevolgd door een dubbbel punt, dan een waarde (*value*) en eindigt met een puntkomma. Bijv. color: red;Waarmee je aanduidt dat de voorgrondkleur of de tekstkleur rood moet zijn.
 - CSS-regels negeren whitespace karakters, je kan dus zoveel spaties, newlines, tabs enz. gebruiken als je wil. Standaard gaan we ook hier de code indenteren voor een betere leesbaarheid.
 - Na de puntkomma kan je een volgende regel zetten die op dezelfde selector toegepast moet worden.
 - Tenzij anders gespecifieerd erven kind-elementen (in de meeste omstandigheden) de CSS-regels van hun ouder-elementen. Zo kan je regels die voor alle elementen moeten gelden makkelijk toepassen op het html-element, want dat is de voorouder van alle andere elementen. (Op de overerving van CSS-regels komen we later nog uitgebreid terug, de volledige werkelijkheid is een stuk complexer.)

### Kleur van h1 aanpassen

Als we nu de kleur van je h1-element aanpassen naar #f04c25 (de hexadecimale RGB-waarde voor Thomas-More-rood) en de grootte naar 24 pixels, krijg je dit in je head:

<style> h1 { color: #f04c25; font-size: 24px; }</style>
## Thomas-More-stijl

Je krijgt een overzichtstabel met de selectoren, de properties en de values die je nodig hebt om onze versie van de Thomas-More-stijl toe te passen. Pas je HTML-document op basis hiervan aan, sla het op en probeer uit.

Probeer op basis van de namen ook uit te vinden wat elke eigenschap doet. Voel je vrij om wat te experimenteren.

 <table style="border-style: solid; border-color: #009cab;" border="1">
    <thead>
        <tr style="background-color: #009cab;">
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">element</span></td>
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">property</span></td>
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">value</span></td>
        </tr>
    </thead>
    <tbody>
        <tr style="background-color: #ccc;">
            <td style="width: 33.3333%; height: 53px;"><span style="color: #000000;">html</span></td>
            <td style="width: 33.3333%; height: 53px;">
                <div>
                    <div><span style="color: #000000;">font-family</span></div>
                </div>
            </td>
            <td style="width: 33.3333%; height: 53px;">
                <div>
                    <div><span style="color: #000000;">"Source Sans Pro", Arial, "Helvetica Neue", Helvetica,</span></div>
                    <div><span style="color: #000000;">sans-serif;</span></div>
                </div>
            </td>
        </tr>
        <tr style="height: 29px;">
            <td style="width: 33.3333%; height: 116px;" rowspan="4"><span style="color: #000000;">h1</span></td>
            <td style="width: 33.3333%; height: 29px;">
                <div>
                    <div><span style="color: #000000;">font-size</span></div>
                </div>
            </td>
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">24px</span></td>
        </tr>
        <tr style="height: 29px;">
            <td style="width: 33.3333%; height: 29px;">
                <div>
                    <div><span style="color: #000000;">line-height</span></div>
                </div>
            </td>
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">26px</span></td>
        </tr>
        <tr style="height: 29px;">
            <td style="width: 33.3333%; height: 29px;">
                <div>
                    <div><span style="color: #000000;">color</span></div>
                </div>
            </td>
            <td style="width: 33.3333%; height: 29px;">
                <div>
                    <div><span style="color: #000000;">#f04c25</span></div>
                </div>
            </td>
        </tr>
        <tr style="height: 29px;">
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">font-weight</span></td>
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">600</span></td>
        </tr>
        <tr style="background-color: #ccc;">
            <td style="width: 33.3333%; height: 116px;" rowspan="4"><span style="color: #000000;">h2</span></td>
            <td style="width: 33.3333%; height: 29px;">
                <div>
                    <div><span style="color: #000000;">font-size</span></div>
                </div>
            </td>
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">18px</span></td>
        </tr>
        <tr style="background-color: #ccc;">
            <td style="width: 33.3333%; height: 29px;">
                <div>
                    <div><span style="color: #000000;">line-height</span></div>
                </div>
            </td>
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">20px</span></td>
        </tr>
        <tr style="background-color: #ccc;">
            <td style="width: 33.3333%; height: 29px;">
                <div>
                    <div><span style="color: #000000;">color</span></div>
                </div>
            </td>
            <td style="width: 33.3333%; height: 29px;">
                <div>
                    <div><span style="color: #000000;">#009cab</span></div>
                </div>
            </td>
        </tr>
        <tr style="background-color: #ccc;">
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">font-weight</span></td>
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">normal</span></td>
        </tr>
        <tr>
            <td style="width: 33.3333%;" rowspan="5"><span style="color: #000000;">p</span></td>
            <td style="width: 33.3333%; height: 29px;">
                <div>
                    <div><span style="color: #000000;">font-size</span></div>
                </div>
            </td>
            <td style="width: 33.3333%;"><span style="color: #000000;">14px</span></td>
        </tr>
        <tr>
            <td style="width: 33.3333%; height: 29px;">
                <div>
                    <div><span style="color: #000000;">line-height</span></div>
                </div>
            </td>
            <td style="width: 33.3333%;"><span style="color: #000000;">20px</span></td>
        </tr>
        <tr>
            <td style="width: 33.3333%; height: 29px;">
                <div>
                    <div><span style="color: #000000;">color</span></div>
                </div>
            </td>
            <td style="width: 33.3333%;"><span style="color: #000000;">#111111</span></td>
        </tr>
        <tr>
            <td style="width: 33.3333%; height: 29px;"><span style="color: #000000;">font-weight</span></td>
            <td style="width: 33.3333%;"><span style="color: #000000;">300</span></td>
        </tr>
        <tr>
            <td style="width: 33.3333%;"><span style="color: #000000;">width</span></td>
            <td style="width: 33.3333%;"><span style="color: #000000;">960px</span></td>
        </tr>
    </tbody>
</table>
<p>&nbsp;</p>
<table style="width: 100%; border-collapse: collapse; border-style: none;" border="1">
    <tbody>
        <tr>
            <td style="width: 8%; border-color: #009cab; background-color: #009cab; text-align: center; vertical-align: middle;"><span style="font-size: 48px;">🚸</span></td>
            <td style="border-style: solid; border-color: #009cab; text-align: left; vertical-align: middle;">
                <p>Pas als je echt vastloopt, mag je naar de broncode van <a href="http://larsderichter.be/user-interfaces/module-1/beetjestijl.html">mijn voorbeeldpagina</a> kijken.</p>
            </td>
        </tr>
    </tbody>
</table>
