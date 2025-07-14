

- Apple Search Ads
-  SearchEntity 

Object

# SearchEntity

The list of geolocations that includes the geoidentifier and entity type.

Search Ads 2.0+

``` source
object SearchEntity
```

## Properties

`adminArea`

`string`

A state or the equivalent according to its associated country.

`countryOrRegion`

`string`

The geoterritory where you’re promoting your app in ISO alpha-2 country code format.

`displayName`

`string`

The geographic targeting location in the format of `locality`,`adminArea,countryOrRegion`.

`entity`

`string`

The type of geography for targeting locations. Search results are in the preferred language according to your organization.

`id`

`string`

The geographic location in the format of CountryOrRegion\|`adminArea`\|`locality`.

`locality`

`string`

A city or the equivalent according to its associated `adminArea`.

## Discussion

Use the Search for Geolocations endpoint to fetch a `displayName` for a geolocation.

### Example Search Entity Object

```
{
  "id": "US|CA|Cupertino",
  "entity": "locality",
  "displayName": "Cupertino, California, United States",
  "countryOrRegion": "US",
  "adminArea": "CA",
  "locality": "Cupertino"
}
```

## See Also

### Search Geolocation Request and Response Objects

object GeoRequest

The geosearch request object.

object SearchEntityListResponse

The response details of geosearch requests.

