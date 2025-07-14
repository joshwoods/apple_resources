

- Apple Search Ads
-  LocalityCriteria 

Object

# LocalityCriteria

The defined targeted audience by locality.

Search Ads 2.0+

``` source
object LocalityCriteria
```

## Properties

`included`

`[string]`

The dimension to include targeted users by locality. For example, in the United States, a locality dimension is a city.

This parameter doesn’t support the `excluded` attribute.

```
"locality": {
      "included": [
        "US|CA|Cupertino"
      ]
    },
```

## Discussion

A `locality` is a city or the equivalent according to its associated `adminArea`.

Use the Search for Geolocations endpoint with the `entity` query parameter to search for and retrieve geolocations. Then use geotargeting dimensions `country`, `adminArea`, and `locality` with Create an Ad Group and Update an Ad Group endpoints.

## See Also

### Audience Refinement

object TargetingDimensions

The optional criteria to use with ad groups to narrow the audience that views your ads.

object AppCategoryCriteria

The defined target audience by app category.

object AppDownloaderCriteria

The defined targeted audience according to app downloads.

object AdminAreaCriteria

The defined targeted audience by administrative area.

object CountryCriteria

The defined targeted audience by country or region.

object AgeCriteria

The defined targeted audience to include using the age demographic.

object AgeRange

The defined target audience to include using the age-range demographic.

object DaypartCriteria

The defined targeted audience to include for a specific time of day.

object DaypartDetail

The defined targeted audience to include by a specific time of day.

object DeviceClassCriteria

The defined targeted audience to include by device type.

object GenderCriteria

The defined targeted audience to include using the gender demographic.

