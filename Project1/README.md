# Nayarit Shelter Locator

This project was devolped for my *Computacional Statistics* course, and I worked alongside my fellows and friends [Carlos López](https://github.com/kennyldc) and [Fernando Miñaur](https://github.com/Fminaurol). 

## Description 

Mexico is a country that due to is location suffers a lot of natural disasters such as earthquakes and hurricanes. In 2021 the states of Nayarit and Sinaloa were hit by *[Hurricane Pamela](https://www.elfinanciero.com.mx/estados/2021/10/16/huracan-pamela-deja-mas-de-10-mil-damnificados-en-nayarit-y-sinaloa/)* affecting more than 10 thousand people; therefore is important to have a tool that helps us to find the nearest shelter in order to help the people in need. The propoused solution was a shiny dashboard.  

The data was stored in a Google Sheet document, therefore the first step was to create an ETL that cleans all the records so that they can be handled in a proper manner. The issues the data had were mainly on the coordinates, as they have diverse special characters. Once the data was clean and ready, was created the dashboard.

The first window of the dashboard displays a table that contains the information of the shelters, it has 3 ways to filter the data, the municipality, address, and type of building. The second window has a map that marks the location of each shelter and it can also be filtered by the municipality. By clicking on the pin all the information is displayed, such as the name of the shelter, address, capacity, and contact information. The last window of the Shiny app displays a map that helps us find the nearest shelter given a certain location, all that is needed is to put a pin in the map and click the button to find the nearest shelter.

In the file [app.R](https://github.com/Juanes8/Juanes8/blob/main/Project1/app.R) is the code of the dashboard as well as the ETL, you can find more details of this project on this [repository](https://github.com/Juanes8/Estadistica-Computacional-fall2021/tree/main/proyectos/RespuestaDesastre/El_bicho_team).

## Packages
- Tidyverse
- Measurements
- Tidyr
- Stringr
- Readxl
- Shiny
- ShinyWidgets
- DT
- Leaflet
- Htmlwidgets
- Shinydashboard
- Geospher