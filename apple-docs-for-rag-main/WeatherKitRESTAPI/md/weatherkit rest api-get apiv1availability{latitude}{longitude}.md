

- WeatherKit REST API
-  GET /api/v1/availability/{latitude}/{longitude} 

Web Service Endpoint

# GET /api/v1/availability/{latitude}/{longitude}

Determine the data sets available for the specified location.

Weather API 1.0.0+

## URL

``` source
GET https://weatherkit.apple.com/api/v1/availability/{latitude}/{longitude}
```

## Path Parameters

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

`country`

`string`

 (Required) 

The ISO Alpha-2 country code for the requested location. This parameter is necessary for air quality and weather alerts.

## Response Codes

` 200 ``OK`

`[`DataSet`]`

`OK`

The request is successful. The data sets are in the response.

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

The server is unable to process the request due to an invalid parameter value.

` 401 ``Unauthorized`

`Unauthorized`

The request isn’t authorized or doesn’t include the correct authentication information.

## See Also

### Obtaining weather information for a location

GET /api/v1/weather/{language}/{latitude}/{longitude}

Obtain weather data for the specified location.

object Weather

The collection of all requested weather data.

type Latitude

A numeric value indicating the latitude of the coordinate between `-90` and `90`.

type Longitude

A numeric value indicating the longitude of the coordinate between `-180` and `180`.

type DataSet

The collection of weather information for a location.

