# Vietnam Market Study - Documentation Site

A comprehensive quantitative analysis and trading guide for Vietnam's stock market, built with Docsify.

## 📊 About This Study

This market study provides in-depth analysis of Vietnam's equity markets for quantitative traders, institutional investors, and market researchers. It covers:

- Macroeconomic landscape and policy environment
- Stock market structure (HOSE, HNX, UPCoM)
- Regulatory framework and foreign ownership limits (FOL)
- Market microstructure and liquidity analysis
- Sector deep-dives and company profiles
- Quantitative analysis and backtesting frameworks
- Trading infrastructure and data sources
- Risk factors and investment opportunities

## 🎯 Target Audience

- **Quantitative Researchers** - Alpha generation strategies
- **Portfolio Managers** - Vietnam allocation decisions
- **Hedge Funds** - Emerging market opportunities
- **Academic Researchers** - Market microstructure studies
- **Active Traders** - Systematic trading approaches

## 📚 Documentation Structure

The study is organized into 9 comprehensive sections:

1. **Executive Summary** - Key findings and actionable recommendations
2. **Market Overview** - Economic landscape and market structure
3. **Regulatory Environment** - FOL, trading rules, reforms
4. **Market Microstructure** - Trading mechanics and liquidity
5. **Sector Analysis** - Banking, Real Estate, Tech, Consumer, Energy, Manufacturing
6. **Quantitative Analysis** - Historical performance, anomalies, risk metrics
7. **Trading Infrastructure** - Data sources, execution, operations
8. **Macro Factors** - Drivers, risks, opportunities
9. **Data & Appendices** - Sources, tables, glossary, contacts

## 🚀 Quick Start

### View Online

**GitHub Pages**: [Your deployment URL will be here]

### Run Locally

**Option 1: Docsify CLI** (Recommended)
```bash
# Install Docsify
npm install -g docsify-cli

# Serve the docs
docsify serve .

# Open http://localhost:3000
```

**Option 2: Python HTTP Server**
```bash
# Python 3
python -m http.server 3000

# Open http://localhost:3000
```

**Option 3: Any Static File Server**
```bash
# Using PHP
php -S localhost:3000

# Using Ruby
ruby -run -ehttpd . -p3000
```

## 📁 File Structure

```
vietnam-market-docs/
├── index.html              # Main configuration & styling
├── home.md                 # Landing page
├── _sidebar.md             # Navigation structure
├── .nojekyll              # GitHub Pages config
│
├── executive-summary/
│   └── executive-summary.md
│
├── market-overview/
│   ├── economic-landscape.md       # ✅ Complete
│   └── stock-market-structure.md   # ✅ Complete
│
├── regulatory/
│   ├── core-regulations.md
│   └── evolving-landscape.md
│
├── microstructure/
│   ├── trading-mechanics.md
│   └── liquidity-metrics.md
│
├── sectors/
│   ├── banking-finance.md
│   ├── real-estate.md
│   ├── consumer-goods.md
│   ├── tech-telecom.md
│   ├── manufacturing.md
│   └── energy.md
│
├── quant/
│   ├── historical-performance.md
│   ├── anomalies-patterns.md
│   └── risk-portfolio.md
│
├── infrastructure/
│   ├── data-sources.md
│   └── execution-operations.md
│
├── macro/
│   ├── macro-drivers.md
│   ├── risks-challenges.md
│   └── opportunities.md
│
└── appendices/
    ├── data-sources.md
    ├── statistical-tables.md
    ├── company-profiles.md
    ├── glossary.md
    └── contacts.md
```

## ✅ Completed Sections

- ✅ Executive Summary (comprehensive)
- ✅ Economic Landscape (detailed with charts/tables)
- ✅ Stock Market Structure (comprehensive)
- 📝 All other sections have templates ready for your content

## 🎨 Features

- **Professional Design** - Financial market aesthetic with IBM Plex fonts
- **Responsive** - Works on desktop, tablet, mobile
- **Full-Text Search** - Search across all documentation
- **Code Highlighting** - Python, R, SQL, JavaScript
- **Table Support** - Data tables with hover effects
- **Navigation** - Easy sidebar navigation with 4 levels
- **Copy Code** - One-click code copying
- **Pagination** - Previous/Next navigation

## 🔧 Customization

### Update Site Name

Edit `index.html`:
```javascript
window.$docsify = {
  name: 'Your Custom Name<span class="app-subtitle">Subtitle</span>',
  // ...
};
```

### Change Colors

Edit CSS variables in `index.html`:
```css
:root {
  --theme-color: #0a4d8f;      /* Primary */
  --accent-color: #c62828;      /* Accent */
  --accent-green: #2e7d32;      /* Success */
  /* ... */
}
```

### Add Content

All content files are markdown (`.md`). Edit them with any text editor:
- Use standard Markdown syntax
- Add tables, lists, code blocks
- Include images: `![alt](path/to/image.png)`

## 📊 Adding Data & Charts

### Tables

```markdown
| Metric | Value | Trend |
|--------|-------|-------|
| GDP Growth | 6.5% | ↑ |
| Inflation | 3.2% | ↔ |
```

### Code Examples

````markdown
```python
import pandas as pd
data = pd.read_csv('vietnam_data.csv')
returns = data['Close'].pct_change()
```
````

### Badges

```markdown
<span class="badge badge-quant">Quantitative</span>
<span class="badge badge-macro">Macro</span>
<span class="badge badge-risk">Risk</span>
<span class="badge badge-data">Data</span>
```

## 🌐 Deployment

### GitHub Pages

1. **Push to GitHub**
```bash
git init
git add .
git commit -m "Initial Vietnam Market Study"
git remote add origin https://github.com/CHAN084ntu/vietnam-market-study.git
git push -u origin main
```

2. **Enable GitHub Pages**
   - Go to repository Settings
   - Pages section
   - Source: main branch / (root)
   - Save

3. **Access**: `https://CHAN084ntu.github.io/vietnam-market-study/`

### Alternative Platforms

- **Netlify**: Drag and drop folder
- **Vercel**: Import from GitHub
- **GitLab Pages**: Use `.gitlab-ci.yml`

## 📚 Data Sources

This study incorporates data from:

**Market Data**:
- Bloomberg Terminal
- Refinitiv Eikon
- SSI iBoard
- VNDIRECT

**Official Sources**:
- State Securities Commission (SSC)
- General Statistics Office (GSO)
- State Bank of Vietnam (SBV)

**Research**:
- Dragon Capital Research
- Academic studies
- World Bank, IMF, ADB reports

## 🤝 Contributing

Contributions welcome! To add content:

1. Fork the repository
2. Edit the relevant `.md` files
3. Test locally with `docsify serve`
4. Submit a pull request

## 📝 License

This documentation template is open source. Market data and analysis content may have separate licensing.

## 📧 Contact

For questions or suggestions:
- GitHub Issues: [Create an issue](https://github.com/CHAN084ntu/vietnam-market-study/issues)
- Email: [Your email]

## 🔄 Updates

**Last Updated**: February 2025

This is a living document. Check back for updates as market conditions and regulations evolve.

---

**Built with**: [Docsify](https://docsify.js.org/) | **Fonts**: [IBM Plex](https://www.ibm.com/plex/)
