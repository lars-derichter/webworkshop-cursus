# 📘 Wat zijn HTML-elementen en HTML-tags?

Als je nog eens terugkijkt naar de HTML-code, vallen 2 zaken op:

- het is een gewoon tekstbestand,
- het lijkt het wel alsof het vol staat met random punthaken of _brackets_ in het Engels **<** en **>**. Uiteraard zijn die niet random en hebben die voor je browser een belangrijke functie en betekenis.

## Elementen

Een webpagina is opgebouwd uit verschillende elementen zoals paragrafen, titels en tussentitels, afbeelding enz. Een element bevat vaak andere elementen (bijv. een paragraaf waarin een woord staat met meer nadruk) en/of het heeft een inhoud (meestal in de vorm van tekst.

## Tags

HTML-elementen worden gemarkeerd met tags:

- Tags beginnen met een ‘opening bracket’: `<`
- gevolgd door de naam van de tag bijv. `p`
- en eindigen met een ‘closing bracket’: `>`

```html
<p>
```

### Closing tags

Op enkele uitzonderingen na staat tekst (of andere inhoud) steeds tussen een ‘opening tag’ (bijv. <p>) en een ‘closing tag’ (bijv. </p>):

- Een ‘closing tag’ begint met een 'opening bracket' gevolgd door een 'forward slash’: `</`
- dan de naam van de tag (bijv. `p`)
- en eindigt met een ‘closing bracket’ `>`

```html
</p>
```
### Volledige tag met inhoud

```html
<p>Dit is een paragraaf</p>
```

### Tags nesten

Je kan ook tags ‘nesten’ of in elkaar steken (zoals Rusissche matroesjka popjes). Dan moet je wel opletten dat je ze in de juiste volgorde sluit, telkens van binnen naar buiten.

bijv.:

```html
<p><strong>Dit is een belangrijke paragraaf.</strong></p>
```

**Verkeerd:**

```html
<p><strong>Dit is een belangrijke paragraaf.</p></strong>
```

### Tags zonder inhoud

Er bestaan ook lege tags. Tas die geen inhoud hebben, maar die informatie bevatten die belangrijk is voor de browser (door middel van attributen, zie verder) of die als placeholder dienen (bijv. voor een afbeelding). Zij hebben (in principe) geen closing tag nodig. Vaak zie je dat webontwikkkelaars ze laten eindigen met `/>` in plaats van `>`. Op zich is dat een goede gewoonte, maar het moet niet in HTML5 (in XML en dus ook in XHTML 4, de voorloper van HTML5 was dat verplicht).

Bijv:

```html
<meta charset="UTF-8" />
```

## Whitespace

De browser negeert alle vormen van ‘whitespace’ (spaties, returns...). Je kan dus al je markup zomaar aan elkaar plakken. Dat betekent ook dat wanneer je een return in je tekst zet, de browser daar geen nieuwe lijn begint.

Voor de leesbaarheid van je code hebben we de gewoonte om die te ‘indenteren’: geneste block tags (zie verder) zetten we op een nieuwe lijn en laten we inspringen met 2 spaties. Ook de bijbehorende closing tags komen dan op een nieuwe lijn en laten we 2 spaties uitspringen. Zo blijft alles goed leesbaar.

Een goede tekst editor helpt je daarbij.
