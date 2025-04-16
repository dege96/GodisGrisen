# 🐷 GodisGrisen

Ett modernt GUI-komponentbibliotek med lekfulla gooey-effekter, byggt med ren HTML, CSS och JavaScript. Inspirerat av godisens mjuka, flytande former!

![GodisGrisen Logo](assets/logo.png)

## ✨ Funktioner

- 🎨 Moderna, animerade GUI-komponenter
- 🫧 Unika gooey-effekter med SVG-filter
- 📱 Helt responsiv design
- 🎯 Lätt att implementera
- 🎪 Lekfull och modern design

### Komponenter
- 🔘 Knappar (primära och sekundära)
- ✅ Checkboxes med gooey-animation
- 🔵 Radio buttons med mjuka övergångar
- 📝 Text inputs med frostat glas-effekt
- 📋 Select/dropdown med anpassad styling

## 🚀 Kom igång

### Installation

1. Klona repot:
```bash
git clone https://github.com/dege96/GodisGrisen.git
```

2. Inkludera filerna i ditt projekt:
```html
<link rel="stylesheet" href="styles.css">
<script src="script.js"></script>
```

### Grundläggande användning

```html
<!-- Knapp -->
<button class="gooey-button primary">Klicka här</button>

<!-- Checkbox -->
<label class="gooey-checkbox">
  <input type="checkbox">
  <span class="checkmark"></span>
  Markera mig
</label>

<!-- Radio button -->
<label class="gooey-radio">
  <input type="radio" name="radio-group">
  <span class="radio-mark"></span>
  Välj mig
</label>

<!-- Text input -->
<input type="text" class="gooey-input" placeholder="Skriv något...">

<!-- Select -->
<select class="gooey-select">
  <option>Välj ett alternativ</option>
</select>
```

## 🎨 Anpassning

### Färger
Du kan enkelt anpassa färgschemat genom att ändra CSS-variabler:

```css
:root {
  --background-color: #ffa726;  /* Bakgrundsfärg */
  --text-color: #eae1e1;       /* Textfärg */
  --accent-color: #d71258;     /* Accentfärg för knappar etc. */
}
```

### Gooey-effekt
SVG-filtret kan justeras för olika grader av "gooeyness":

```html
<filter id="goo">
  <feGaussianBlur in="SourceGraphic" stdDeviation="8" result="blur" />
  <feColorMatrix in="blur" mode="matrix"
    values="1 0 0 0 0  
            0 1 0 0 0  
            0 0 1 0 0  
            0 0 0 30 -15" result="goo" />
  <feComposite in="SourceGraphic" in2="goo" operator="atop"/>
  <feGaussianBlur stdDeviation="1" result="endBlur"/>
</filter>
```

## 🛠️ Teknisk information

- Inga externa beroenden
- Byggd med vanilla JavaScript
- Använder moderna CSS-funktioner:
  - CSS Custom Properties (variabler)
  - Flexbox för layout
  - CSS Grid för komponenter
  - SVG-filter för gooey-effekter

## 📱 Browser-stöd

- ✅ Chrome (senaste)
- ✅ Firefox (senaste)
- ✅ Safari (senaste)
- ✅ Edge (senaste)

## 🤝 Bidra

1. Forka repot
2. Skapa en feature branch (`git checkout -b feature/AmazingFeature`)
3. Committa dina ändringar (`git commit -m 'Add some AmazingFeature'`)
4. Pusha till branchen (`git push origin feature/AmazingFeature`)
5. Öppna en Pull Request

## 📝 Todo

- [ ] Lägg till fler komponenter
- [ ] Skapa en komponentdokumentation
- [ ] Implementera dark mode
- [ ] Lägg till fler animationer
- [ ] Skapa en demo-sida

## 📜 Licens

Distribuerad under MIT-licensen. Se `LICENSE` för mer information.

## 👋 Kontakt

Daniel Egelrud - [@dege96](https://github.com/dege96)

Projektlänk: [https://github.com/dege96/GodisGrisen](https://github.com/dege96/GodisGrisen) 