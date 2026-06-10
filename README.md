# Woon Langer Thuis — Website

Simpele statische website voor woonlangerthuis.nl. Gebouwd met pure HTML, CSS en minimaal JavaScript. Geen framework, geen database.

## Bestandsstructuur

```
woonlangerthuis/
├── index.html          Homepage + blogoverzicht
├── over-mij.html       Over mij pagina
├── nieuwsbrief.html    Nieuwsbrief aanmeldpagina
├── contact.html        Contactpagina
├── style.css           Alle stijlen (één bestand)
├── blog/
│   ├── woningaanpassingen-toekomstproof.html
│   ├── zelesta-dekbedovertrek.html
│   └── gps-tracker-dementie.html
└── README.md
```

## Hoe voeg je een nieuw blogartikel toe?

### Stap 1 — Kopieer een bestaand artikel
Kopieer één van de bestaande blogbestanden in de `/blog/` map en geef het een nieuwe naam. Gebruik een beschrijvende bestandsnaam met koppeltekens, zonder spaties of speciale tekens. Bijvoorbeeld: `subsidie-woningaanpassing-aanvragen.html`

### Stap 2 — Pas de metatags aan (in de `<head>`)
```html
<title>Jouw artikeltitel — Woon Langer Thuis</title>
<meta name="description" content="Korte omschrijving van het artikel (max. 160 tekens).">
```

### Stap 3 — Pas de hero-kleur aan
Kies een categoriekleur door de juiste CSS-klasse te gebruiken op de `.blog-post-hero` div:
- `cat-woningaanpassingen` — bruingrijs
- `cat-zorgtechnologie` — teal
- `cat-subsidies` — paars
- `cat-mantelzorg` — groen
- `cat-productadvies` — terra (oranje)

### Stap 4 — Vul het artikel in
Vervang de titel, datum, categorie-label en de inhoud van `.blog-content`.

### Stap 5 — Voeg het artikel toe aan de homepage
Open `index.html` en voeg een blogkaartje toe aan de `.blog-grid` sectie. Kopieer een bestaand `<article class="blog-card">` blok en pas de tekst, link en klasse aan.

---

## MailerLite koppelen

De nieuwsbriefsectie (`nieuwsbrief.html`) bevat een HTML-formulier als placeholder. Vervang dit door de embed-code van MailerLite:

1. Ga in MailerLite naar **Forms → Embedded forms**
2. Maak een nieuw formulier aan (minimaal: voornaam + e-mail)
3. Kopieer de embed-code
4. Vervang het `<form>` blok in `nieuwsbrief.html` door de MailerLite code
5. Verwijder ook het JavaScript onderaan dat het nep-bevestigingsbericht toont

---

## Hosting

Upload alle bestanden via FTP naar je webhosting. Zorg dat `index.html` in de root staat. Geen server-side configuratie nodig — het zijn gewoon statische bestanden.

**Aanbevolen hosting voor statische sites:** Netlify (gratis), Cloudflare Pages (gratis), of gewone gedeelde hosting via bijv. TransIP of Antagonist.

---

## Kleuren (voor referentie)

| Naam | Hex |
|---|---|
| Terra (primair) | `#C0845A` |
| Bruin (secundair) | `#7B3F1E` |
| Achtergrond | `#FDFAF6` |
| Tekstkleur | `#333333` |
| Accentgroen | `#7AAE8A` |
| Licht terra | `#f5ebe1` |
