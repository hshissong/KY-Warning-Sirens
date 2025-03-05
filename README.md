# KY-Warning-Sirens
A project mapping known locations of outdoor warning sirens in Kentucky created by Hannah Hissong for University of Kentucky in February-March 2025

Must include:
Active link to the final index.html page
 The README.md file will be visualized at the pathway following the pattern *https://github.com/username/repository-name*
 The index.html file will be visualized at *https://username.github.io/repository-name*. 
 You will need to create links on each page that links to the other page. For example, creating a link on the README.md file that takes the viewer to the index.html page.

## Project Contents

If you wanted to include a table of contents to sections, and then links to each section.

- [Data Source](#data-source)
- [Project Background](#project-background)
- [Mapmaking Process](#mapmaking-process)
- [Map Summary](#map-summary)

***

### Data Source

[Link to Fayette county data source](https://data.lexingtonky.gov/datasets/eab218eb4e2249d59a39401b5ee25d6e/explore)

[Link to metro Louisville data source](https://jefferson-ky-outdoor-warning-sirens-lojic.hub.arcgis.com/) 
Cody Ashbaugh at Louisville Metro Emergency Services supplied additional data for Jefferson, Shelby, Bullitt, Spencer, and Oldham counties. Many thanks to him for this work!
Most data around Cincinnati and the outliers across the state came from Open Street Map

Many sirens for smaller towns or rural counties write out a description of the location on a website such as: "Danville Fire Department Station 1 (Main Street)". While this information is helpful for local residents who go searching for that specific information, it is not helpful for a statewide or national initiative or database. Collecting all written locations like this across the state of Kentucky was outside the scope of realistic work to take on for this project but would make an excellent research project and case for further study.

Some lists are managed by cities but most appear to be managed by counties. Some local National Weather Service offices in other parts of the country keep a list of sirens they know about but most just include general information about the use of sirens. Sirens are not set off remotely by a national or even local network which is why there was not a complete dataset I could locate for this project. Instead most of them are set off singularly leading to a host of problems. Because sirens are not set off as a group, there has been no need to assemble a database of their locations across a state or the entire nation. Most are managed by the county emergency response teams which is why most of the listings seem to be managed by counties. 

### Project Background and Purpose

Outdoor warning sirens are commonly, though mistakenly, relied upon to alert people to incoming dangerous weather. The hypothesis for this project is that there are not enough outdoor warning sirens spread across the Commonwealth of Kentucky for that to be a reliable way for residents to expect weather warnings. I set out to create a map showing all outdoor warning sirens across the state and how far sound from those sirens could reasonably extend from the location of the siren. According to the government of Boone County, Missouri (https://www.showmeboone.com/oem/resources/sirens.asp) outdoor warning sirens can reliably be heard at a distance of one mile, so that is the measure used in this project. Other sources varied between half a mile and up to five miles, so one mile, found most commonly, was used in this project. Again, another potential area of study after this project would be to gain a clearer understanding of how far that sound is reasonably able to travel from the location of the siren. A range of 0.5 to 5.0 miles leaves a large margin of error when lives are on the line. 

### Mapmaking Process

I used a basemap from Open Street Map to draw attention to the most prominent natural and urban features across Kentucky. Being able to see this data along with the siren positions help illustrate why so many sirens are clustered around particular areas and why I had trouble finding siren data for more rural locations. I then did several google searches using search terms like "outdoor warning siren locations kentucky" to find any publicly availalbe data. As discussed above, there wasn't much. I emailed the National Weather Service office in Louisville to ask if they kept any data, and they directed me to Cody at Louisville Emergency Managment Services. He emailed me a CSV file of the data linked above which I imported to QGIS along with the data I found from Fayette county. Additionally I did a Quick OSM query for "key siren:type" and all values to get additional data tagged as sirens in Open Street Map. Finally, at the encouragement of Louisville Emergency Management Services, I emailed the Kentucky Emergency Management office to ask for any data they have but did not receive a reply in time for this project. 

After importing all the siren data I could find, I drew a one mile buffer (using the Buffer tool under Vector geometry in the Processing Toolbox in QGIS) around each siren to demonstrate how far sound from that siren could reliably reach in an emergency. Additionally I added an outline for the state of Kentucky to show where the boundaries exist in this data. 
 
* Final Map projection: EPSG:3089

### Map summary

At a state level, the outlook is bleak. Much of this map is empty because I was not able to find data on where warning sirens exist outside of the three major metropolitan areas of the state. Within each of those cities, though, the data is more encouraging, so additional maps zoomed in to each of the three urban areas are also included. Much of the Lexington and Louisville metro areas could reasonably expect to hear a warning siren when it is set off. The data on the Kentucky side of Cincinnati is a little more spread out meaning not every person in that metro area has as good a chance to hear a siren as someone in Louisville or Lexington, but that data is relying on what users have tagged in Open Street Map so it may be incomplete. 

## Final Project Link

Here you are linking from the README.md to the index.html.

Please view the [final map online](www.github...)
