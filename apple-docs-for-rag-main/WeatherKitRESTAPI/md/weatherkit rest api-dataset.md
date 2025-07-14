

- WeatherKit REST API
-  DataSet 

Type

# DataSet

The collection of weather information for a location.

Weather API 1.0.0+

``` source
string DataSet
```

## Possible Values 

`currentWeather`  

`forecastDaily`  

`forecastHourly`  

`forecastNextHour`  

`weatherAlerts`  

## Attributes 

Possible types:

## Possible Values

currentWeather  
The current weather for the requested location.

forecastDaily  
The daily forecast for the requested location.

forecastHourly  
The hourly forecast for the requested location.

forecastNextHour  
The next hour forecast for the requested location.

weatherAlerts  
Weather alerts for the requested location.

## See Also

### Obtaining weather information for a location

GET /api/v1/availability/{latitude}/{longitude}

Determine the data sets available for the specified location.

GET /api/v1/weather/{language}/{latitude}/{longitude}

Obtain weather data for the specified location.

object Weather

The collection of all requested weather data.

type Latitude

A numeric value indicating the latitude of the coordinate between `-90` and `90`.

type Longitude

A numeric value indicating the longitude of the coordinate between `-180` and `180`.

