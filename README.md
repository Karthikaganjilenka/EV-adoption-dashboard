# Global EV Adoption and Market Trends Visualization

The transition to electric vehicles is one of the most significant shifts in modern transportation. But how fast is it actually happening, where is it happening, and what does it tell us about the future of oil dependence? This project sets out to answer those questions visually — not with tables or reports, but through an interactive dashboard built to let anyone explore the data themselves.

Using over a decade of global EV data (2010 to 2024), we designed and built a series of interactive D3.js visualizations hosted on Observable. The result is a dashboard where policymakers, researchers, and curious readers can trace the rise of electric vehicles across countries, compare powertrain preferences, and see in real numbers how much oil the EV revolution has already displaced.

---

## Live Dashboard

Explore the interactive visualizations here:  
[Observable Dashboard](https://observablehq.com/d/840ed787c4e40ff8)

---

## The Dataset

**Source:** Kaggle — Global EV Sales 2010–2024 (originally from IEA)  
**Coverage:** 2010 to 2024 across countries and regions worldwide

Each row in the dataset captures a specific metric — EV sales, EV stock, EV sales share, or oil displacement — broken down by region, year, vehicle mode (cars, buses, vans, trucks), and powertrain type (BEV, PHEV, or FCEV). Before any visualization could happen, the data needed cleaning: missing and empty values were removed, only analytically useful parameters were retained, and numerical consistency was enforced throughout.

---

## What We Built

The dashboard is organized around six core questions about global EV adoption. Each question drives a visualization designed to give a direct, honest answer.

**How have global EV sales grown over time?**  
A line chart tracking total EV sales from 2010 to 2024 reveals a curve that was nearly flat for the first half of the decade, then bent sharply upward after 2020, reaching approximately 14 million vehicles sold by 2023. The growth is not gradual — it is exponential.

**Which vehicle types are growing fastest?**  
A multi-line chart breaks the stock data down by vehicle category — cars, buses, vans, and trucks — on a log scale. Cars dominate at every point, but the gap between categories has been narrowing since around 2015, with vans and trucks beginning to close ground.

**How do powertrain preferences vary between the US and the rest of the world?**  
Donut charts comparing the US against all other regions reveal a meaningful difference. Outside the US, Battery Electric Vehicles (BEVs) hold 42% of the market. Inside the US, that share drops to 24%, with a notably higher proportion of general EVs and FCEVs. The US market has not consolidated around BEVs to the same degree as other leading regions.

**Which powertrain type dominates globally?**  
A log-scale bar chart of cumulative vehicle counts makes the answer clear: BEVs account for roughly 280 million units globally, PHEVs for around 130 million, and FCEVs remain a distant third at approximately 830,000. The BEV is not just leading — it is the market.

**Where in the world is EV adoption highest?**  
A choropleth map of EV stock by country as of 2023 shows concentration in China, the United States, and parts of Western Europe — with France standing out as one of the most significant European hubs. Much of Africa, South Asia, and Latin America remain at early-stage adoption levels.

**Is EV growth actually reducing oil dependence?**  
A grouped bar chart comparing EV sales against oil displacement year by year shows that the two have moved together — as EV adoption climbed, so did the volume of oil displaced. The relationship is consistent, suggesting that the environmental impact of EV adoption, while still smaller in scale than total oil demand, is measurable and growing.

---

## Project Structure

```
EV-adoption-dashboard/
├── IEA Global EV Data 2024.csv                                      # Source dataset
├── Electric Vehicles Adoption & Market Trends Visualization.pdf     # Final report
├── Project_design.pdf                                               # Visualization design document
├── final_project_proposal.pdf                                       # Project proposal
└── cis671_project__presentation.pptx                               # Class presentation
```

---

## Tech Stack

D3.js · Observable · Python · Pandas

Data preprocessing was handled in Python using Pandas. All six interactive visualizations were built in D3.js and published on the Observable platform.

---

## Team

**Course:** CIS 671 — Information Visualization, Grand Valley State University  
**Instructor:** Prof. Haoyu Li

