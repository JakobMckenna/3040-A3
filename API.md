# 3040 Assignment 3 - Part one
## Manitoba weather API
### Description: 
##### The Manitoba weather API gives information on the current weather in a variety of places around Manitoba based on given location data such as latitude, longitude, and postal code. The API can also return past data based on a date paramater being passed to it along with location data. There are a variety of paramaters returned based on which endpoint you are accessing. 

### Endpoint and paramaters

#### Endpoint 1: The user can get the type of weather anywhere in Manitoba by entering three paramaters: longitude, latitude, and a date.

#### Paramaters: 
##### Lat(float)
##### Long(float)
##### Date(string)

##### The user can get the weather of any location in Manitoba based on the Latitude/Longitude and Date they enter.

#### Endpoint 2: The user can get the weather details based on the postal code. 

#### Paramater: 
##### postal_Code(string)

#### The user can get a variety of weather details based on a given postal code.

### Description of resources (JSON)

#### Endpoints:
#### GET: GET /weatherType
#### GET: GET /weatherType/{postalArea}/windSpeed
#### GET: GET /weatherType/{postalArea}/humidty

#### {
  "resources": [
    {
      "name": "manitobaWeather",
      "endpoints": [
        {
          "method": "GET",
          "url": "/weatherType",
          "description": "Returns the type of weather for these coordinates"
        },
        {
          "method": "GET",
          "url": "/products/{postalCode}",
          "description": "Returns details of weather based on a postal code"
        },
       ]
    }
   ]
   

### Response and return

#### Sample request:

##### https://api.manitobaweather.org/json?lat=lat=53.760&lng=long=98.8139&date=2023-03-15

#### Sample response:

##### {
      "results":
      {
        "weather":"sunny",
        "wind_kph": "16.7",
        "humidity": "51"
     
      },
       "status":"OK"
    }
