---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<meta http-equiv='cache-control' content='no-cache'> 
<meta http-equiv='expires' content='0'> 
<meta http-equiv='pragma' content='no-cache'>

<header>
    <h1> A statistical insight into drug/narcotic crimes in SF in the years 2003 to 2017.</h1>
    <p> By: Anders Thuesen, Anne Desler, Linea Bartholdy </p>
    <p> Date: 23-03-2023 </p>
</header>

<h2>
    The data
</h2>

This article concerns the data set: <a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry">Police Department Incident Reports: Historical 2003 to May 2018.</a> The data contains extensive information about more than two million crime incidents from San Francisco in the years 2003 to 2018. Each registered incidents the dataset includes eg. category of crime, exact location and time. In total the data concerns 37 different categories. This article crime specifically focuses on the crime "Drug/Narcotics" to give a valuable insight into the patterns of drug related crimes in the city. Since 2018 is incomplete this investigation only concerns the years up to and including 2017. In the considered time period, the police registered 116352 incidents in this category which is the 6th highest number of occurrences of crimes in the data. Hereby drugs/narcotics related crimes accounts for 6% of the total number of crimes.

<h2>
    Data analysation and visualization
</h2>

A more in depth investigation of the data leads to the discovery of a clear pattern throughout the day and week. In figure 1 the number of occurrences are plotted on a weekly basis showing the 168 hours of the week.  

<figure>
<center>
    <img src="/figures/timeseries_plot.png" width="600" height="300" label>
    <figcaption>Figure 1 - Plot of occurences of Drug/Narcotics crimes in the 168 hours of the week.</figcaption>
</center>
</figure>

In figure 1 it is observed from the registered incidents that the number of drug-related incidents are least frequent around 6am in the morning and increases steadily throughout the day. The number of occurrences are systematically most frequent around 4pm in the afternoon and decreases during the afternoon and night. 
<br>
<br>
However in order to obtain a more specific overview of where the drug related crimes are registered the following map provides the number of occurrences within the different districts of San Francisco. 

<figure>
<center>
    {% include map_plot.html %}
    <figcaption>Figure 2 - Map of occurences in diffeent districts of San Francisco.</figcaption>
</center>
</figure>

In figure 2 the number of incidents are compensated for the area of the district. Hence the number of incidets are multiplied by the area of the district divided by the total area of San Francisco. Hereby the number of occurrences can be compared across districts with large variation of size. On the map it is observed that the Southern district has the highest number of registered occurrences. This number of this district is significantly higher than any other district and implies a high presence of drugs in the district. In general drug related crimes are significantly more present in the northern part of the city. 