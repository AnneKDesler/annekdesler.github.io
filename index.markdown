---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<meta http-equiv='cache-control' content='no-cache'> 
<meta http-equiv='expires' content='0'> 
<meta http-equiv='pragma' content='no-cache'>

<header>
    <h1> A statistical insight into drug/narcotic crimes in San Francisco in the years 2003 to 2017.</h1>
    <p> By: Anders Thuesen (s183926), Anne Desler (s194333), Linea Bartholdy (s185231)</p>
    <p> Date: 27-03-2023 </p>
</header>

<h2>
    The data
</h2>

This article concerns the dataset: <a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry">Police Department Incident Reports: Historical 2003 to May 2018.</a> The data contains extensive information about more than two million crime incidents from San Francisco in the years 2003 to 2018. For each registered incident the dataset includes eg. the category of crime, exact location, and time. In total, the data concerns 37 different crime categories. This article specifically focuses on the crime "Drug/Narcotic" to give valuable insight into the patterns of drug-related crimes in the city. Since the year 2018 is incomplete this investigation only concerns the years up to and including 2017. In the considered time period, the police registered 116352 incidents in the drugs category which is the 6th highest number of occurrences of crimes in the dataset. Hereby drugs/narcotics-related crimes account for 6% of the total number of crimes.

<h2>
    Data analysis and visualization
</h2>

A more in-depth investigation of the data leads to the discovery of a clear pattern throughout the day and week. In figure 1 the number of occurrences is plotted on a weekly basis showing the 168 hours of the week.  

<figure>
<center>
    <img src="/figures/timeseries_plot.png" width="600" height="300" label>
    <figcaption>Figure 1 - Plot of occurrences of Drug/Narcotic crimes in the 168 hours of the week.</figcaption>
</center>
</figure>

In figure 1 it is observed that the number of drug-related incidents is least frequent around 6 in the morning and increases steadily throughout the day. The number of occurrences is systematically most frequent around 4 in the afternoon and decreases during the afternoon and night. 
<br>
<br>
However, to obtain a more specific overview of where the drug-related crimes are registered we provide a map showing the number of occurrences within the different districts of San Francisco. 

<figure>
<center>
    {% include map_plot.html %}
    <figcaption>Figure 2 - Map of drug/narcotic related crime occurrences in different districts of San Francisco.</figcaption>
</center>
</figure>

In figure 2 the number of incidents is compensated for the area of the district. Hence the number of incidents is multiplied by the area of the district divided by the total area of San Francisco. Hereby the number of occurrences can be compared across districts with a large variation in size. On the map, it is observed that the Southern district has the highest number of registered occurrences. The number of incidents in this district is significantly higher than in any other district and implies a high presence of drugs in the district. In general drug-related crimes are significantly more present in the middle and northern parts of the city. 