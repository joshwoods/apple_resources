

- WeatherKit REST API
-  Longitude 

Type

# Longitude

A numeric value indicating the longitude of the coordinate between `-180` and `180`.

Weather API 1.0.0+

``` source
number Longitude
```

## Attributes 

Minimum: `-180`

Maximum: `180`

Possible types:

## Discussion

Negative values indicate west of the prime meridian; positive values indicate east of the prime meridian.

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

type DataSet

The collection of weather information for a location.

