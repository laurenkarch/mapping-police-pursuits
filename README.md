# mapping-police-pursuits
Final project for MAP 671 course. Maps traffic fatalities involving police pursuits from 2016-2020 and suggests mapping as a tool to further study pursuit-related fatalities.

# Mapping Police Pursuits: Dear Statehouse, It&#39;s Leslie Again

## **The Issue**

Between 2016 and 2020, police pursuits were involved in [1,903](https://cdan.dot.gov/SASStoredProcess/guest) fatal motor vehicle crashes that killed 2,209 people. Despite an average death count of 442 people per year—including officers, suspects, and bystanders—data about police pursuits is scant. Statewide pursuit law is varied and often insubstantial, consigning high-risk-reward decisions to individual jurisdictions or, more often, individual officers. Ohio law, for example, requires only that law enforcement agencies maintain a pursuit policy—the state makes no recommendation regarding that policy&#39;s contents.

I&#39;ve created two maps for this project, both relating to fatalities involving law enforcement vehicular pursuits: an overview map, and a suggestion on mapping future data.

## **Mapping Fatal Chases**

The first map shows the coordinates of motor vehicle fatalities involving police pursuit from 2016 to 2020. This data comes from the [National Highway Traffic Safety Administration&#39;s Fatality and Injury Reporting System Tool (FIRST).](https://cdan.dot.gov/query)

NHTSA defines a police pursuits as: &quot;an event that is initiated when a law enforcement officer, operating an authorized emergency vehicle, gives notice to stop (either through the use of visual or audible emergency signals or a combination of emergency devices) to a motorist who the officer is attempting to apprehend, and that motorist fails to comply with the signal by either maintaining his/her speed, increasing speed, or taking other evasive action to elude the officer&#39;s continued attempts to stop the motorist.&quot; NHTSA data is pulled from police reports.

The national map was created in QGIS 3.22.5, and projected in North America Lambert Conformal Conic - ESRI:102009. A base map showing state boundaries was created using [Census TIGER data](https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html). Information on states with the highest and lowest per-capita pursuit fatality rates uses [2020 Census data](https://www.census.gov/programs-surveys/decennial-census/decade/2020/2020-census-results.html) to determine the population denominator.

## **Suggestions for Mapping Pursuit Data**

In 2016, Ohio&#39;s governor and district attorney assembled a task force of legislators and law enforcement experts to advance recommendations regarding police pursuit policy. [Its recommendations include a call for improved data collection](https://www.ohioattorneygeneral.gov/Files/Briefing-Room/News-Releases/Policy-and-Legislation/Vehicular-Pursuit/AGLEVP-Special-Report-November-2016-w-links.aspx):

_&quot;Absent the requirement to forward reports of vehicle crashes to the Ohio Department of Transportation, there is no requirement of law enforcement agencies in the state to report all vehicle pursuits. There is also no central state database for agencies to voluntarily provide vehicle pursuit information. Accordingly, it is recommended that such a data collection site be initiated and maintained, and that collected data be analyzed to further develop best practices in this law enforcement activity.&quot;_

Since 2016, no such database has been developed.

This recommendation may be difficult to implement, in part because of the nature of police pursuits in the state. Not only do police departments work together to continue chases, officers may travel beyond the bounds of their jurisdictions under mutual aid agreements. The NHTSA collects data on the location of fatal crashes, but no national or state agency compiles data on pursuit routes.

The local map proposes a concept for illustrating police chases through mapping, using a single fatal chase as an example.

On December 6, 2021, police in Solon, Ohio, pursued a Ford Fusion that has been reported stolen at gunpoint. According to a [press release](https://twitter.com/SolonPolice/status/1467932763454164996) from the department, officers pursued the suspect northbound at high speeds through nearby Bentleyville and into Chagrin Falls before losing the car. According to a police report from Chagrin Falls, Chagrin Falls followed the Fusion for several blocks at non-pursuit speed, and contacted Solon police when it headed southbound toward Solon again. Solon officers deployed Stop Sticks near the point of the chase&#39;s origin. The driver of the Fusion, traveling at approximately 85 miles per hour, hit the Stop Sticks and crashed into two nearby vehicles. The crash injured two people and killed the 85-year-old passenger of one of the bystander vehicles.

Ideally, a database regarding pursuit routes would include the following attributes:

- An incident ID referencing all units involved in a single incident
- Paths of police vehicles, including coordinates and distances
- Condition information, including time of day and weather
- Maximum and average speeds
- Suspect information, including potential charges and vehicle type
- Use of tire deflation devices

This map was created in QGIS 3.22.5, and projected in NA83/ Ohio North, EPSG: 3734. The basemap uses [OpenStreetMap data](https://www.openstreetmap.org/#map=18/40.03986/-84.20450) for roadways and [Census TIGER data](https://catalog.data.gov/dataset/tiger-line-shapefile-2016-state-ohio-current-county-subdivision-state-based) for municipal boundaries. The location of the crash comes from NHTSA data, and pursuit routes are digitized from the Solon press release and the Chagrin Falls police report.
