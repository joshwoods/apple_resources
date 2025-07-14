

- WeatherKit REST API
-  Weather 

Object

# Weather

The collection of all requested weather data.

Weather API 1.0.0+

``` source
object Weather
```

## Properties

`currentWeather`

CurrentWeather

The current weather for the requested location.

`forecastDaily`

DailyForecast

The daily forecast for the requested location.

`forecastHourly`

HourlyForecast

The hourly forecast for the requested location.

`forecastNextHour`

NextHourForecast

The next hour forecast for the requested location.

`weatherAlerts`

WeatherAlertCollection

Weather alerts for the requested location.

## Attributes 

Possible types:

## See Also

### Obtaining weather information for a location

GET /api/v1/availability/{latitude}/{longitude}

Determine the data sets available for the specified location.

GET /api/v1/weather/{language}/{latitude}/{longitude}

Obtain weather data for the specified location.

type Latitude

A numeric value indicating the latitude of the coordinate between `-90` and `90`.

type Longitude

A numeric value indicating the longitude of the coordinate between `-180` and `180`.

type DataSet

The collection of weather information for a location.

