

- Apple Search Ads
-  GeoRequest 

Object

# GeoRequest

The geosearch request object.

Search Ads 2.0+

``` source
object GeoRequest
```

## Properties

`entity`

`string`

 (Required) 

The type of geography for targeting locations. Search results are in the preferred language according to your organization.

Possible Values: `AdminArea, Country, Locality`

`id`

`string`

 (Required) 

The geographic location in the format of CountryOrRegion\|`adminArea`\|`locality`. A `countryCode` is an ISO alpha-2 country code string. An `adminArea` is a state or the equivalent according to its associated `country`. A `locality` is a city or the equivalent according to its associated `adminArea`.

Use the `id` that returns in the response in the TargetingDimensions object.

## See Also

### Search Geolocation Request and Response Objects

object SearchEntity

The list of geolocations that includes the geoidentifier and entity type.

object SearchEntityListResponse

The response details of geosearch requests.

