# mapping-police-pursuits
Final project for MAP 671 course. Maps traffic fatalities involving police pursuits from 2016-2020 and suggests mapping as a tool to further study pursuit-related fatalities.

I created two maps for this project, both relating to fatalities involving law enforcement vehicular pursuits: an overview map, and a suggestion on mapping future data.

## **National Map**

The first map shows the coordinates of motor vehicle fatalities involving police pursuit from 2016 to 2020. This data comes from the [National Highway Traffic Safety Administration&#39;s Fatality and Injury Reporting System Tool (FIRST).](https://cdan.dot.gov/query)

The national map was created in QGIS 3.22.5, and projected in North America Lambert Conformal Conic - ESRI:102009. A base map showing state boundaries was created using [Census TIGER data](https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html). Information on states with the highest and lowest per-capita pursuit fatality rates uses [2020 Census data](https://www.census.gov/programs-surveys/decennial-census/decade/2020/2020-census-results.html) to determine the population denominator.

## **Suggestions for Mapping Pursuit Data**

The local map proposes a concept for illustrating police chases through mapping, using a single fatal chase as an example.

This map was created in QGIS 3.22.5, and projected in NA83/ Ohio North, EPSG: 3734. The basemap uses [OpenStreetMap data](https://www.openstreetmap.org/#map=18/40.03986/-84.20450) for roadways and [Census TIGER data](https://catalog.data.gov/dataset/tiger-line-shapefile-2016-state-ohio-current-county-subdivision-state-based) for municipal boundaries. The location of the crash comes from NHTSA data, and pursuit routes are digitized from the Solon press release and the [Chagrin Falls police report](/Incident2100428.PDF).
 ![final poster](/poster8000.png)
