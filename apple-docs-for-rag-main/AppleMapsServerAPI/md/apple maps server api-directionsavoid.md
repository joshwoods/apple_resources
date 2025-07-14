

- Apple Maps Server API
-  DirectionsAvoid 

Type

# DirectionsAvoid

A list of the features you can request to avoid when calculating directions.

Apple Maps Server API 1.2+

``` source
string DirectionsAvoid
```

## Possible Values 

`Tolls`  

## Possible Values

Tolls  
When you set `avoid=Tolls`, routes without tolls are higher up in the list of returned routes. Note that even when you set `avoid=Tolls`, the routes the server returns may contain tolls (if no reasonable toll-free routes exist). Ensure you check the value of `routes[i].hasTolls` in the response to verify toll assumptions.

## See Also

### Getting common type information

type CountryCode

A string that represents a two-letter country code.

type Lang

A string that represents a standard tag for identifying languages.

type PoiCategory

A string that describes a specific point of interest (POI) category.

type SearchLocation

A string that describes a geographic location in the form of longitude and latitude.

type SearchRegion

A string that describes a region to search in terms of its upper-right and lower-left corners as a pair of geographic points.

type UserLocation

A string that describes the user’s location in terms of longitude and latitude.

