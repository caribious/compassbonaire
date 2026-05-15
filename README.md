# 🧭 Compass Bonaire Website

Welkom bij het GitHub repository van **Compass Bonaire** - uw gids voor het ontdekken van het eilandparadijs!

## 📋 Inhoud

Dit repository bevat de volledige website voor compassbonaire.com:

- **index.html** - Volledige Nederlandse website
- **styles.css** - Modern responsief design met animaties
- **script.js** - Interactieve features en formuliervalidatie
- **.github/workflows/deploy.yml** - Automatische deployment naar TransIP

## 🚀 Deployment naar TransIP

### Vereisten:

1. GitHub Secrets ingesteld (zie hieronder)
2. Actieve TransIP account met FTP-toegang

### GitHub Secrets Configuratie:

Voeg deze 3 secrets toe in **Repository Settings → Secrets and variables → Actions**:

| Secret | Beschrijving | Voorbeeld |
|--------|-------------|----------|
| `FTP_SERVER` | TransIP FTP-server adres | `ftp.transip.nl` |
| `FTP_USERNAME` | TransIP FTP-gebruikersnaam | `username@compassbonaire.com` |
| `FTP_PASSWORD` | TransIP FTP-wachtwoord | `your-secure-password` |

### Automatische Deployment:

Zodra je een commit pusht naar de `main` branch, zal GitHub Actions automatisch:
1. ✅ Je code uitchecken
2. ✅ Verbinding maken met je TransIP FTP-server
3. ✅ De bestanden uploaden
4. ✅ De website live zetten

## 🛠️ Lokale Development

Voor lokale testing:

1. Clone het repository:
```bash
git clone https://github.com/caribious/compassbonaire.git
cd compassbonaire
```

2. Open `index.html` in je browser
3. Maak wijzigingen naar wens
4. Test in je browser (F5 om te refreshen)
5. Commit en push naar GitHub

## 📝 Bestandsstructuur

```
compassbonaire/
├── index.html           # Hoofdwebsite
├── styles.css          # Styling
├── script.js           # JavaScript functionaliteit
├── .gitignore          # Git ignore regels
├── .github/
│   └── workflows/
│       └── deploy.yml  # Deployment workflow
└── README.md           # Dit bestand
```

## 🎨 Website Features

- ✨ Responsive design (werkt op telefoon, tablet, desktop)
- 🎭 Smooth animations en transitions
- 📧 Contactformulier met validatie
- 🧭 Sticky navigatie
- 📱 Mobile-friendly UI
- ⚡ Scroll animaties

## 💡 Tips voor Development

### Wijzigingen aanpassen:
- **Kleuren veranderen?** Bewerk `styles.css`
- **Inhoud toevoegen?** Bewerk `index.html`
- **Functionaliteit?** Update `script.js`

### Live Deployment:
```bash
git add .
git commit -m "Update website content"
git push origin main
# GitHub Actions zal automatisch deployen!
```

## 📞 Ondersteuning

Voor vragen of problemen:
1. Check je GitHub Secrets zijn correct ingesteld
2. Verificeer je TransIP FTP-credentials
3. Check de workflow run logs in GitHub Actions

## 📄 Licentie

© 2026 Compass Bonaire. Alle rechten voorbehouden.

---

**Veel plezier met het ontwikkelen van compassbonaire.com! 🏝️**