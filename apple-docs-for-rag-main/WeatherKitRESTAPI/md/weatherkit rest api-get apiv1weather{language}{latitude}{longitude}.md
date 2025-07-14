

- WeatherKit REST API
-  GET /api/v1/weather/{language}/{latitude}/{longitude} 

Web Service Endpoint

# GET /api/v1/weather/{language}/{latitude}/{longitude}

Obtain weather data for the specified location.

Weather API 1.0.0+

## URL

``` source
GET https://weatherkit.apple.com/api/v1/weather/{language}/{latitude}/{longitude}
```

## Path Parameters

`language`

`string`

 (Required) 

The language tag to use for localizing responses.

`latitude`

Latitude

 (Required) 

The latitude of the desired location.

Minimum: `-90`

Maximum: `90`

`longitude`

Longitude

 (Required) 

The longitude of the desired location.

Minimum: `-180`

Maximum: `180`

## Query Parameters

`countryCode`

`string`

The ISO Alpha-2 country code for the requested location. This parameter is necessary for weather alerts.

`currentAsOf`

`date-time`

The time to obtain current conditions. Defaults to `now`.

`dailyEnd`

`date-time`

The time to end the daily forecast. If this parameter is absent, daily forecasts run for 10 days.

`dailyStart`

`date-time`

The time to start the daily forecast. If this parameter is absent, daily forecasts start on the current day.

`dataSets`

`[`DataSet`]`

A comma-delimited list of data sets to include in the response.

`hourlyEnd`

`date-time`

The time to end the hourly forecast. If this parameter is absent, hourly forecasts run 24 hours or the length of the daily forecast, whichever is longer.

`hourlyStart`

`date-time`

The time to start the hourly forecast. If this parameter is absent, hourly forecasts start on the current hour.

`timezone`

`string`

 (Required) 

The name of the timezone to use for rolling up weather forecasts into daily forecasts.

## Response Codes

` 200 ``OK`

Weather

`OK`

The request is successful. The weather alert is in the response.

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

The server is unable to process the request due to an invalid parameter value.

` 401 ``Unauthorized`

`Unauthorized`

The request isn’t authorized or doesn’t include the correct authentication information.

## See Also

### Obtaining weather information for a location

GET /api/v1/availability/{latitude}/{longitude}

Determine the data sets available for the specified location.

object Weather

The collection of all requested weather data.

type Latitude

A numeric value indicating the latitude of the coordinate between `-90` and `90`.

type Longitude

A numeric value indicating the longitude of the coordinate between `-180` and `180`.

type DataSet

The collection of weather information for a location.

