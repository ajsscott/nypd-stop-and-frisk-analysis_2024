# Analyzing Racial Disparities in NYPD ‘Level 3’ Stop-and-Frisk Civilian Interactions

## Background
Although a federal court found the New York City Police Department’s abusive stop-and-frisk practices [unconstitutional](https://www.theguardian.com/world/2013/aug/12/new-york-stop-and-frisk-unconstitutional-judge) over a decade ago, reform attempts have failed and the NYPD is still accused of continuing its [discriminatory practices](https://www.cityandstateny.com/opinion/2023/07/opinion-nypds-stop-and-frisk-practices-are-still-here-under-new-name/388627/) today. Right now, the NYPD can approach anyone they want and ask questions like what their name is or where they’re going – what the NYPD classifies as  “Level 1 or 2” stops - for *any* reason, or none at all. The person is under no obligation to respond to such requests, and according to the NYPD patrol guide, "may refuse to answer questions or walk or even run away".

These Level 1 or 2 encounters are some of the most common interactions between officers and New Yorkers. And because they don’t rise to the level of a "stop-and-frisk" (considered Level 3 stops) – when officers must have “reasonable suspicion” of criminal activity – the NYPD has not been required to track or publicly report on any of these encounters.

The police are already under a federal requirement to collect and share detailed information about ‘Level 3’ stops, when the police have a stronger suspicion that a person has committed a crime and an officer may use “reasonable force” to stop a person, ask “accusatory” questions and frisk the person. The [How Many Stops Act](https://www.nytimes.com/2024/02/03/nyregion/nypd-how-many-stops-act.html) requires that officers now provide similar information for lesser ‘Level 1’ and ‘Level 2’ stops, including noting the reason for any inquiry, demographic details about the person being stopped and why the stop was made.

In January 2024, the New York City Council voted to override [Mayor Eric Adams’s veto](https://www.nytimes.com/2024/01/30/nyregion/adams-veto-police-solitary.html) to enact the **How Many Stops Act**, which requires police officers to record the race, age and gender of most people they approach. Critics of the bill claim the bill doesn't really combat unbiased policing. “When I was a captain, I was the commanding officer of two precincts. The 81st and the 113th. Both in African-American communities, 90% of the people who were stopped in those communities were African American. If you go to Middle Village and do the stops, 97% of the people there are Caucasian. ‘So, what have you proved?’” Wilbur Chapman, a former NYPD chief of patrol and deputy commissioner, said to the [NY 1 Sepctrum News](https://ny1.com/nyc/all-boroughs/politics/2024/02/02/what-comes-next-for-the--how-many-stops-act--) in February 2024.

## Research Question
Immediately prior the **How Many Stops Act** implementation (which is ongoing), what are the demographic and geospatial allocations of current ‘Level 3’ or ‘Stop-and-Frisk’ civilian interactions? Are these numbers significant enough to indicate racial or geographic bias, even before considering the Level 1 and Level 2 interaction data the How Many Stops Act will provide?

## Project Goal
-   Analyze ‘Level 3’ stop-and-frisk data from recent years by racial, gender and location markers
- Use the findings to conclude whether recent NYPD history shows compelling evidence for racial and location-based bias in stop-and-frisk interactions.

## Data Needs & Sources:
-   Stop-And-Frisk Data:
    -   Publicly available [NYPD Stop, Question, and Frisk database](https://www.nyc.gov/site/nypd/stats/reports-analysis/stopfrisk.page)
    -   [ACLU Analysis of Stop-and-Frisk History](https://www.nyclu.org/en/stop-and-frisk-data)
-   City Data:
    -   Neighborhood Limits and Police Districts
    -   Demographic breakdown of city, preferably as geospatial data


## Analysis
-   Use Python libraries like Pandas, NumPy, and SciPy to conduct statistical analysis:
    -   Calculate stop-and-frisk rates by race and location
    -   Analyze the association between race and stop outcomes (citations, searches, arrests).
    -   Perform sentiment analysis on arrest records to compare phrasing
    -   Determine if those associations are significant enough to indicate bias
-   Map the data to geospacial visualizations, comparing stops of income, racial breakdown of neighborhoods.
    -   Compare stop rates to neighborhood demographics and general population distributions. Are police stopping black people more in mostly white neighborhoods? Are police patrolling high income neighborhoods more or less? Are they stopping people when they do patrol more or less? How do the demographics of those people that they stop compare to the demographics of the neighborhood overall.

## Results
-   Make conclusions on bias based on analysis
-   Visualize  plots and graphics to support statistical conclusions