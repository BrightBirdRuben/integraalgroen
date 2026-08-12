# Integraal Groen — website (prototype)

## Testen
Pak de zip uit en dubbelklik op `index.html`. De site opent lokaal in je browser — geen server nodig. Klik door de navigatie, test het hamburgermenu op mobiel (of verklein je browserscherm).

## Pagina's
- `index.html` — homepage
- `zorg.html`, `bedrijven.html`, `vastgoed.html`, `scholen.html`, `publieke-sector.html` — de vijf doelgroeppagina's
- `groendirect.html` — Groen Direct landingspagina
- `style.css` — alle opmaak (kleuren, lettertypes, lay-out) — één centraal bestand voor alle pagina's
- `assets/logo.png` — het logo

## Teksten aanpassen
Elke pagina is gewone HTML. Open een bestand met een teksteditor (bv. Kladblok, TextEdit, VS Code) en pas de tekst tussen de tags aan, bijvoorbeeld:
```html
<h1>Uw buitenomgeving.<br>Integraal beheerd.</h1>
```
Verander gewoon de tekst tussen `<h1>` en `</h1>`. Sla op en herlaad de pagina in je browser.

## Foto's toevoegen
Op de plekken waar een foto moet komen, staat nu een groen blok met een label zoals:
```html
<div class="photo-placeholder"><span class="tag">Foto: zorgomgeving</span></div>
```
Vervang dit door een echte afbeelding:
1. Zet je foto in de `assets`-map, bv. `assets/zorg-hero.jpg`.
2. Vervang het blok door:
```html
<img src="assets/zorg-hero.jpg" alt="Beschrijving van de foto" style="width:100%; aspect-ratio:4/5; object-fit:cover; border-radius:12px;">
```
Voor de grote banners bovenaan de doelgroeppagina's (`photo-banner`) geldt hetzelfde principe, maar met `aspect-ratio:16/6`.

## Kleuren en lettertypes aanpassen
Bovenaan `style.css` staat een blok met alle kleuren:
```css
:root{
  --white:#FFFFFF;
  --green-deep:#153A2C;
  --green-fresh:#5B9C4C;
  --grey-warm:#F6F4F0;
  --ink:#33362F;
}
```
Verander een hex-code en de hele site past zich overal aan — je hoeft niet door elke pagina te zoeken.

## Nog te doen
- Echte foto's plaatsen (zie hierboven)
- De knoppen ("Vraag een terreinbezoek aan", "Meld een buitenprobleem") linken naar een echt contactformulier of de Groen Direct-bestelmodule
- Contactgegevens (adres, telefoon, e-mail) toevoegen in de footer en de contactsectie
- Het citaat op de Zorg-pagina vervangen door een echte referentie zodra die er is
