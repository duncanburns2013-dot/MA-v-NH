<p align="center">
  <img src="social-card.png" alt="MA vs NH — One Border, Two Economies" width="100%"/>
</p>

# MA vs NH: One Border, Two Economies

**A data-driven competitiveness analysis of Massachusetts and New Hampshire using exclusively federal government data sources.** No media rankings, no think-tank scores — just the numbers.

> _"Massachusetts ranks #1 in the nation on education... but 6 in 10 students don't meet grade-level expectations on the state's own test."_

---

## 🔴 Live Dashboard

**[→ View the interactive dashboard](https://duncanburns2013-dot.github.io/MA-v-NH/)**

Built as a single-file HTML dashboard with 16 interactive Chart.js visualizations, animated counters, crosshair hover effects, and a dark editorial design aesthetic.

---

## Key Findings

### Labor Market
- **MA unemployment: 4.8%** vs **NH: 3.1%** (Dec 2025, SA) — MA now *above* the national average (4.4%)
- New England payroll employment growth: **0%** (Nov 2024–2025)
- MA declined **−0.1%** annualized in Q1 2025 vs US +1.4%

### Economic Output — Total vs Per Capita
- MA GDP per capita **$110.6K** (#2 nationally) — genuinely high output per person
- MA total PCE growth **5.3%** (#1 nationally) — but inflated by population growth (+66K international immigrants)
- **Per capita**, the gap narrows dramatically:
  - PCE growth: MA 4.2% vs NH 3.9% (0.3pp gap, not 0.9pp)
  - **Per capita income growth: NH leads MA — +3.5% vs +3.3%**
- MA spent **~$932M in FY2024** on emergency shelters under the right-to-shelter law (~half migrant families). This is government consumption, not PCE — but new residents' household spending inflates total PCE mechanically

### The Income Illusion
- A $100K earner retains:
  - **$87,769** in purchasing power in MA (5% income tax + 8.2% higher prices)
  - **$103,093** in NH (0% income tax + 3% lower prices)
  - **$15,324 real advantage for NH (17.5%)**
  - *Note: MA's 9% rate only applies to income above ~$1.08M (Fair Share surtax)*

### Migration — NH Flipped
- NH flipped to **net positive domestic migration** in 2024: **+6,843** (was −7,058 in 2023)
- MA→NH corridor **nearly doubled**: 9,024 net flow in 2024 vs 4,854 in 2023
- MA domestic outflow improved but remains deeply negative: **−30,553**
- MA relies on international immigration (+66,158) to offset domestic losses

### Education — Behind the Rankings
- MA is **#1 on NAEP** (national test) — but that's because every state struggles; MA just struggles less
- **MCAS Reality (MA's own test):** Only **39% ELA** and **41% math** proficiency in grades 3–8
- **Pandemic collapse:** ELA dropped from 52% (2019) → 39% (2024). Grade 10 math: 59% → 45%
- **Gateway Cities divide:** Affluent suburbs (Weston, Lexington) score **72–82%** vs working-class cities (Lawrence, Holyoke) at **9–18%**
- UMass Donahue Institute: **84% of MCAS score variation** explained by socioeconomic factors
- MA voters **repealed MCAS** as graduation requirement (Question 2, Nov 2024)

---

## Data Sources — Government Only

| Agency | Dataset | Vintage |
|--------|---------|---------|
| **BLS** | LAUS (unemployment), CES (payroll), QCEW (wages), JOLTS | Dec 2025 / Q3 2025 |
| **BEA** | GDP by State, RPP, Real PCE & PI (SARPI) | 2024 (released Feb 19, 2026) |
| **Census** | ACS State-to-State Migration Tables | 2021–2024 |
| **NCES** | NAEP 2024, CCD School Finance FY22 | 2024 |
| **MA DESE** | MCAS Achievement Results | Spring 2024 & 2025 |
| **NEA** | Rankings & Estimates 2023–24 | 2024 |
| **UMass** | Donahue Institute (MCAS variance study) | Cited |
| **MA Admin** | Emergency Assistance Shelter Reports | FY2024–25 |

**No data from:** CNBC Top States, US News rankings, Tax Foundation, Cato, any think tank index, or media composite scores.

---

## Technical Details

- **Single-file HTML** — no build step, no dependencies to install
- **Chart.js 4.4** via CDN for all 16 visualizations
- **Interactive features:** Crosshair hover, index-mode tooltips, animated counters, year-toggle migration flow diagram, tab navigation with scroll
- **Design:** Dark editorial aesthetic (Playfair Display + DM Sans + JetBrains Mono), neon accent palette (#ff2d2d, #00bfff, #00ff88, #ffcc00, #ff7700)
- **Responsive** — works on desktop and mobile

### Run Locally

```bash
git clone https://github.com/duncanburns2013-dot/MA-v-NH.git
cd MA-v-NH
open index.html
```

### Deploy to GitHub Pages

Enable Pages in repo settings → Source: `main` branch, root (`/`).

---

## Methodology Notes

- All unemployment figures are **seasonally adjusted** (BLS LAUS, released Jan 27, 2026)
- PCE and PI figures are **real** (inflation-adjusted) from BEA's SARPI tables
- Migration uses **Census ACS state-to-state flow tables** (direct bilateral counts, not estimates)
- RPP (Regional Price Parities) from BEA/FRED — MA 108.238, NH ~97.0 (2023 vintage)
- MCAS data from MA DESE official achievement reports — Gateway Cities figures are illustrative district-level examples
- Income Illusion calculation: $100K gross → apply state income tax → divide by RPP/100 → real purchasing power
- Question 2 (MCAS repeal) may affect 2025+ test-taking effort — noted in dashboard caveats

---

## Contributing

Found a data error? Have a newer vintage? Open an issue or PR. This project prioritizes accuracy over narrative.

---

## License

MIT

---

<p align="center">
  <sub>Built with federal data, Chart.js, and a commitment to showing what the numbers actually say.</sub>
</p>
