# 3040 Assignment 3 - Part one
## Manitoba weather API
### Description: 
##### The Manitoba weather API gives information on the current weather in a variety of places around Manitoba based on a given latitude and longitude. 

### Endpoint and paramaters
#### Endpoint: The user can get the type of weather anywhere in Manitoba by entering three paramaters: longitude, latitude, and a date.
##### https://api.manitobaweather.org/com/latlongdate/123?&lat=53.7609&long=98.8139&date=2020-07-16
#### Paramaters: 
##### Lat(float)
##### Long(float)
##### Date(string)

##### The user can get the weather of any location in Manitoba based on the Latitude/Longitude and Date they enter.

#### Endpoint: The user can get the weather details based on four paramaters: wind speed, humidity, cloud, and postal code. 
##### https://api.manitobaweather.org/com/weatherdetail/123?&Lwind_kph=14.9&humidity=60&cloud=50
#### Paramaters: 
##### Lwind_kph(float)
##### humidity(float)
##### cloud(float)
##### postal_Code(string)

### Description of resources 

### Response and return
#### Sample request:
##### https://api.manitobaweather.org/json?lat=lat=53.760&lng=long=98.8139&date=2023-03-15
#### Sample response:
##### {
      "results":
      {
        "weather":"sunny",
        "Lwind_kph": "14.8",
        "humidity": "61",
        "cloud": "50"
     
      },
       "status":"OK"
    }
