

- WeatherKit REST API
-  Latitude 

Type

# Latitude

A numeric value indicating the latitude of the coordinate between `-90` and `90`.

Weather API 1.0.0+

``` source
number Latitude
```

## Attributes 

Minimum: `-90`

Maximum: `90`

Possible types:

## Discussion

Negative values indicate south of the equator; positive values indicate north of the equator.

## See Also

### Obtaining weather information for a location

GET /api/v1/availability/{latitude}/{longitude}

Determine the data sets available for the specified location.

GET /api/v1/weather/{language}/{latitude}/{longitude}

Obtain weather data for the specified location.

object Weather

The collection of all requested weather data.

type Longitude

A numeric value indicating the longitude of the coordinate between `-180` and `180`.

type DataSet

The collection of weather information for a location.

