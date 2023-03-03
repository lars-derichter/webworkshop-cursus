# 📘 Een beetje tekstopmaak

We overlopen hier een aantal veelgebruikte css-properties om tekst op te maken. De uitleg zal nogal basic zijn, maar voor meer details kan je steeds terecht op de [CSS reference van het Mozilla Developer Network.](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

## font-family

Het lettertype dat je wil gebruiken. Dit kan de naam van een lettertype zijn of een lijst van namen, waarbij het systeem eerst zoekt naar het eerste lettertype en als dat niet gevonden wordt op het systeem overgaat naar het volgende etc. Meestal sluit je af met één van de generieke font-families (serif, sans-serif etc.) als ultieme fallback. Als de naam een spatie bevat, zet je hem best tussen aanhalingstekens.

```css
html { 
    font-family: "Source Sans Pro", Arial, "Helvetica Neue", Helvetica,sans-serif;
}
```

## font-size

De grootte van het lettertype voor een bepaald element. Dit kan uitgedrukt worden in [alle CSS-lengtematen](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units#Lengths), maar de meest eenvoudige voor nu is px voor pixels.

```css
h1 { 
    font-size: 24px;
}
```

## line-height

De hoogte van een lijn tekst. De line-height - de font-size = de witruimte tussen twee regels tekst. it kan uitgedrukt worden in [alle CSS-lengtematen](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units#Lengths), maar de meest eenvoudige voor nu is px voor pixels.

```css
p { 
    line-height: 20px;
}
```

## font-style

De ‘stijl’ van een font: normal, italic of oblique.

```css
em { 
    font-style: italic;
}
```
## font-weight

Hoe vet het lettertype is. De waarde is normal of bold of een honderdtal van 100 – 900 waarbij 400 overeenkomt met normal en 700 met bold. 100 is dan zoiets al ultra-thin en 900 zou ook extra-bold kunnen zijn.

```css
p { 
    font-weight: 300
}
```

## color

De kleur van je letters. Kleurwaarden kunnen op heel veel verschillende manieren uitgedrukt worden in CSS. De meest gebruikte zijn hexadecimale RGB-waarden en namen van veel voorkomende kleuren zoals red of green of light-blue. We zullen later nog enkele manieren bekijken, voor een overzicht kan je al eens piepen op de [MDN reference pagina voor color values.](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value)

```css
h1 { 
    color: #f04c25;
}
```

## text-decoration

Bepaalt of een tekstfragment onderlijnd wordt, 'bovenlijnd' of doorgestreept wordt. Waarden zijn: none, underline, overline of linethrough.

```css
a { 
    text-decoration: none;
}
```

 <table style="width: 100%; border-collapse: collapse; border-style: none;" border="1">
    <tbody>
        <tr>
            <td style="width: 8%; border-color: #f04c25; background-color: #f04c25; text-align: center; vertical-align: middle;"><span style="font-size: 36pt;">⚠️</span></td>
            <td style="border-style: solid; border-color: #f04c25; text-align: left; vertical-align: middle;">
                <p>Als je de onderlijning bij links weghaalt, moet je wel op een andere manier duidelijk maken dat het om een link gaat!</p>
            </td>
        </tr>
    </tbody>
</table>
