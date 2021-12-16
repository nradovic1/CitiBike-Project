# CitiBike-Project
<img src="https://cdn.vox-cdn.com/thumbor/xpj5jeGm9D3ZvtkTMXrZJnb0hlo=/0x0:2000x1333/920x613/filters:focal(840x507:1160x827):format(webp)/cdn.vox-cdn.com/uploads/chorus_image/image/65737608/170920_14_05_28_5DS_6462.0.jpg">

## Background
Citi Bike is a privately owned public bicycle sharing system serving the New York City boroughs that was launched in May 27, 2013. Currently, it is the largest bike sharing program in the United States, with 48,315 daily rides and over 17,000 vehicles. The name was given after the lead sponsor of the program, Citi Group, but was bought by Lyft in 2018.

## Purpose
The purpsoe of this project is to create a platform that gives details on every Citi Bike in Manhatten with real-time data from Cti Bike API. Furthermore, we will extract 2020 data from the same API and using Tableau, look at some trends and analyze the ridership program and see where there are opportunities for growth.

## Technologies
* JavaScript (D3.js, Leaflet)
* Python (Pandas)
* HTML/CSS/Bootstrap
* Tableau

## Process

### Real-time Dashboard

1. Used the Citi Bike station information API to get information about the station names and locations. Each object in the `stations` array has `station_id`, `name`, `capacity`, `lat`, and `lon` properties. The [logic.js](logic.js) file contains coordinates that you can use to position a Leaflet map over New York City.

2. Developed code to perform a second API call to the Citi Bike station status API. This is real-time detailed data of all bike stations. This data contains: `station_id`, `num_bikes_available`, `is_installed`, and `is_renting`.

3. Used the data from the second API call to add the following functionality:

    * In the popup for each marker, display the number of available bikes.

    * Added a layer control, and split the markers into the following layer groups:

        * **Coming Soon:** 

        * **Empty Stations:** 

        * **Out of Order:** 

        * **Low Stations:**

        * **Healthy Stations:**

4. Utilized a Leaflet plugin to create different types of markers to represent the bike stations layer. 

5. Added a legend to map to explain the different markers.   

6. Deployed it to GitHub Pages.

Visit at https://nradovic1.github.io/CitiBike-Project/!

### Tableau

Collecting data from Citi Bike API on every ride in 2020 and transforming using Pandas in Jupyter Notebook, I was able to gain a lot of insights into the bike sharing program. Using Tableau, I visualized the data into a Story for excecutives to take make us of and help with decision making.

Please check out the Tableau Story at:
https://public.tableau.com/app/profile/novak.radovic/viz/HW_twbx/CitiBikeAnalysis?publish=yes







