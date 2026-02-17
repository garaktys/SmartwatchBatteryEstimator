# Smartwatch Battery Estimator

Een interactieve web-applicatie om de batterijduur van je smartwatch in te schatten op basis van je gebruikspatroon en apparaattype.

## 🎯 Functionaliteiten

- **Smartwatch type selectie**: Kies tussen Basic (fitness tracker), Standard (smartwatch), Pro (high-end) of Apple Watch Series 11 GPS
- **Batterijcapaciteit invoer**: Configureerbare batterijcapaciteit in mAh (standaard 100-600 mAh range)
- **Actief gebruikspatroon**: Definieer dagelijkse schermtijd en interactie in uren (0-24 uur)
- **Extra verbruik opties**:
  - GPS (workouts en navigatie)
  - Always-on display
  - Veel notificaties (standaard ingeschakeld)
- **Real-time berekening**: Onmiddellijke batterijduurschatting in dagen en uren
- **Gepersonaliseerd advies**: Handige tips gebaseerd op je configuratie

## 📁 Projectstructuur

```
SmartwatchBatteryEstimator/
├── index.html      # HTML-structuur met formulier en resultaatweergave
├── styles.css      # Responsive styling (dark theme, glasmorphisme)
├── app.js          # Berekeningen en logica
├── logo.png        # Logoafbeelding
└── README.md       # Dit bestand
```

## 🚀 Hoe te gebruiken

1. Open `index.html` in je webbrowser
2. Selecteer je smartwatch type uit de dropdown
3. Vul de batterijcapaciteit in (mAh) - gebruik de hint als richtlijn
4. Stel je dagelijkse actieve gebruikstijd in (uren/dag)
5. Vink de van toepassing zijnde extra verbruikopties aan
6. Klik op "Bereken batterijduur"
7. Bekijk je schatting in het resultaatgedeelte met praktische tips

## 🔋 Berekening

De app berekent batterijduur op basis van:

- **Actief verbruik**: Verbruik wanneer scherm aan is (vermenigvuldiger: 1,4x)
- **Standby verbruik**: Achtergrondactiviteit rest van de dag (vermenigvuldiger: 0,6x)
- **Extra vermenigvuldigers**:
  - GPS: +1,5x verbruik
  - Always-on display: +1,3x verbruik
  - Veel notificaties: +1,1x verbruik

**Apparaatprofielen** (mAh per uur):
- Basic: 8 mAh/uur
- Standard: 12 mAh/uur
- Pro: 16 mAh/uur
- Apple Watch Series 11: 16 mAh/uur

## 🎨 Design & UX

- **Dark theme** met glasmorphisme effecten
- **Responsive layout** (Desktop, tablet, mobiel)
- **Accessibility**: ARIA live region voor dynamische resultaten
- **Bereikbare UI**: Duidelijke labels, hints en intuïtieve invoervelden
- **Nederlandse interface** voor Nederlandse gebruikers

## 💻 Technologie

- **HTML5**: Semantische structuur met formuliervalidatie
- **CSS3**: Grid/Flexbox layout, animations, media queries
- **Vanilla JavaScript**: Event handlers, realtime berekeningen

## ⚠️ Disclaimer

Dit is een **demo-applicatie** voor trainings- en educatiedoeleinden. De batterijberekeningen zijn geschat en niet wetenschappelijk bewezen. Gebruik deze schattingen niet voor kritische toepassingen of officiële batterijduurclaims.

## 👤 Auteur

Gemaakt door Casper van Geet als GitHub training project.

## 📄 Licentie

Vrij te gebruiken voor educatiedoeleinden.
