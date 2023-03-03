# 🧪 Een profielfoto

De mens is (over het algemeen) een visueel wezen. Het wereldwijde web kon pas doorbreken bij het grote publiek toen er afbeeldingen aan werden toegevoegd.

Het is de bedoeling dat je nu een profielfoto toevoegt aan je pagina.

## Een afbeelding toevoegen

Er zijn verschillende methoden om afbeeldingen toe te voegen aan een webpagina met HTML. De voorkeursmanier in HTML5 om een op zichzelf staande afbeelding met betekenis in te voegen is als volgt:

```html
<figure> 
    <img src="profielfoto.jpg" alt="Mijn profielfoto" />
</figure>
```
 
<table style="width: 100%; border-collapse: collapse; border-style: none;" border="1">
    <tbody>
        <tr>
            <td style="width: 8%; border-color: #009cab; background-color: #009cab; text-align: center; vertical-align: middle;"><span style="font-size: 36pt;">ℹ️</span></td>
            <td style="border-style: solid; border-color: #009cab; text-align: left; vertical-align: top;">
                <p>Een img-element kan niet op zichzelf voorkomen (het is een inline-element en kan dus enkel voorkomen als child-element van een block-element dat dan als een soort container werkt; later meer hierover).</p>
                <p>Als een afbeelding bedoeld is als (deel van) een illustratie, is <em>figure</em> het meet geschikte container-element om een img-element in te vervatten. Als het een louter decoratieve afbeelding is, kan het betekenisloze <em>div</em> gebruikt worden.</p>
                <p>Maak je geen zorgen als deze paragraaf Chinees voor je is. Dit wordt later wel duidelijk, maar wie al een beetje (meer ouderwetse) HTML heeft geleerd, zou hier over kunnen struikelen. Die mensen moeten voorlopig maar even aannemen dat ik gelijk heb, de uitleg volgt later&hellip;</p>
            </td>
        </tr>
    </tbody>
</table>

### src-attribuut

Het belangrijkste onderdeel van een img-tag is het src-attribuut. Dat bevat de url van het grafische bestand dat weergegeven moet worden. Je merkt dat hier geen http gebruikt wordt en ook geen domeinnaam. Wanneer een bestand zich in dezelfde folder als het html-bestand bevindt, mag je gewoon de naam van het bestand gebruiken (de eenvoudigste vorm van een relatieve url).

In dit geval moet er dus in dezelfde folder als ons index.html bestand een foto zitten met als bestandsnaam profielfoto.jpg.

### alt-attribuut

Niet alle browsers kunnen (steeds) afbeeldingen weergeven. De verbinding kan te traag zijn, de gebruiker werkt misschien met een tekst-browser of het gaat om een slechtziend persoon die een text-to-speech synthesizer gebruikt om het op het web te surfen. Daarvoor dient het alt-attribuut. In al deze gevallen zal de tekst in het alt-attribuut gebruikt worden in plaats van de afbeelding zelf. (En vergeet niet, Google is de grootste blinde gebruiker van het web ook om je ranking in zoekmachines te verbeteren en te zorgen dat je site via Google images etc. gevonden kan worden, speelt het alt-attribuut een belangrijke rol.

### Bestandsformaten

Alle moderne browsers kunnen werken met JPEG-bestanden (extensie .jpg of .jpeg), GIF-bestanden en PNG-bestanden. Er bestaan nog andere bestandsformaten, maar de ondersteuning daarvan is nog niet universeel (looking at you, webp).

## Nu is het aan jou

Zoek een goede profielfoto van jezelf (of een foto van een kitten of puppy, die doen het ook altijd goed) en voeg ze toe tussen je titel en je paragra(a)f(en) met tekst.

<table style="width: 100%; border-collapse: collapse; border-style: none;" border="1">
    <tbody>
        <tr>
            <td style="width: 8%; border-color: #009cab; background-color: #009cab; text-align: center; vertical-align: middle;"><span style="font-size: 36pt;">🚸</span></td>
            <td style="border-style: solid; border-color: #009cab; text-align: left; vertical-align: middle;">
                <p>Als je helemaal vastloopt, kijk dan naar mijn versie: <a href="http://larsderichter.be/user-interfaces/module-1/profielfoto-1.html">http::/www.larsderichter.be/user-interfaces/module-1/profielfoto-1.html</a>.</p>
            </td>
        </tr>
    </tbody>
</table>

## Stijl

Als je nu in je browser kijkt, is je afbeelding heel lastig gepositioneerd.

Voeg het volgende toe binnen de style-tag om je afbeelding mooi, links in je tekst te zetten:

```css
figure { 
    float: left; 
    margin: 0 20px 20px 0;
}
```

 <table style="width: 100%; border-collapse: collapse; border-style: none;" border="1">
    <tbody>
        <tr>
            <td style="width: 8%; border-color: #009cab; background-color: #009cab; text-align: center; vertical-align: middle;"><span style="font-size: 36pt;">🚸</span></td>
            <td style="border-style: solid; border-color: #009cab; text-align: left; vertical-align: middle;">
                <p>Je hoeft dit stukje code nog niet te begrijpen, weet gewoon dat het de afbeelding links zet en dat het de marges rond de afbeelding goed zet.</p>
                <p>Als je vastloopt, bekijk dan mijn voorbeeld: <a href="http://larsderichter.be/user-interfaces/module-1/profielfoto-2.html">http::/www.larsderichter.be/user-interfaces/module-1/profielfoto-2.html</a>.</p>
                <p>Als je foto te groot is, kan je ze best bijwerken met een eenvoudig grafisch programma (<a href="https://support.microsoft.com/nl-be/help/27916/windows-10-edit-photos-videos">in Windows 10 kan dat met de foto&rsquo;s app</a>; <a href="https://support.apple.com/nl-be/guide/preview/prvw2015/mac">in macOS kan dat in preview.</a>)</p>
            </td>
        </tr>
    </tbody>
</table>
