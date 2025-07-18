# Racial Disparities in NYPD ‘Level 3’ Stop-and-Frisk Interactions

![Python Version](https://img.shields.io/badge/python-3.10+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

---

## Quick Links

* **[Final Report (PDF)](./nypd_stop-and-frisk_final_report.pdf)** – Full project findings and statistical analysis.
* **[Data & Code](./notebooks/)** – Python scripts and notebooks for reproducibility.
* **[Visualizations](./reports/figures/)** – Maps and charts highlighting significant racial disparities.

---

## Author
AJ Strauman-Scott
M.S. in Data Science, City University of New York
📍 New York, NY
📫 ajstraumanscott@pm.me
🔗 [LinkedIn](www.linkedin.com/in/ajstraumanscott) • [GitHub](https://github.com/ajsscott)

---

## Background

Despite a 2013 federal court ruling that declared NYPD’s stop-and-frisk practices [unconstitutional](https://www.theguardian.com/world/2013/aug/12/new-york-stop-and-frisk-unconstitutional-judge), analysis of recent **Level 3 stop-and-frisk data** suggests systemic racial bias remains prevalent. These stops—defined as interactions where officers have “reasonable suspicion” and may frisk individuals—are now complemented by expanded reporting requirements under the **[How Many Stops Act](https://www.nytimes.com/2024/02/03/nyregion/nypd-how-many-stops-act.html)**.

Our analysis of 2022–2023 data examined racial and geographic disparities in these Level 3 interactions to assess patterns of bias prior to the act’s implementation.

---

## Research Question

* How do the racial and demographic distributions of Level 3 stops compare to the underlying neighborhood populations?
* Are these disparities statistically significant, indicating systemic bias?

---

## Data Sources

* **NYPD Stop, Question, and Frisk database** ([link](https://www.nyc.gov/site/nypd/stats/reports-analysis/stopfrisk.page)) – Level 3 stop records with detailed demographics and geospatial information.
* **2020 U.S. Census data** – Racial composition by census tract.
* **NYC Open Data GIS layers** – Police precincts and census tract boundaries.

---

## Analysis

* **Chi-Square Goodness-of-Fit Tests** were performed per census tract to evaluate racial distributions of stops against local demographics.
* **Geospatial Integration**: Using GeoPandas, stops were mapped to 2020 census tracts and visualized alongside neighborhood racial data.
* **Conditions for Validity**:

  * Independence of census and stop data was assumed.
  * All tracts had sufficient sample sizes (≥5 expected cases per category).

---

## Key Results

* **Widespread Bias**: Nearly 50% of census tracts showed statistically significant racial disparities (p < 0.05).
* **Extreme Deviations**: Over 90% of significant tracts had p-values close to zero, indicating severe mismatches between the expected racial breakdown (based on population) and those stopped by NYPD.
* **Citywide Impact**: Bias was observed across every borough and precinct, with no evidence that issues were localized to specific “problem areas.”
* **Geospatial Findings**: Visualizations revealed clusters of bias across income-diverse neighborhoods, reinforcing that racial factors dominate stop decisions over geographic or economic factors.

---

## Visualizations

* Heatmaps of census tracts reveal severe racial bias citywide.
* Overlay of precinct boundaries confirms that bias is pervasive across all NYPD precincts.

---

## Conclusion

The analysis shows **systemic racial bias** in NYPD Level 3 stop-and-frisk interactions. Disparities are not limited to a few “bad actors” but appear embedded across the institution, with more than **30,000 Level 3 stops analyzed** reflecting statistically significant bias.

Future research could expand this analysis to Level 1 and Level 2 stops (as new data becomes available) and explore related policing activities, such as traffic stops and arrests, to assess broader systemic trends.

