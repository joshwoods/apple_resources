

- Apple Search Ads
-  AdminAreaCriteria 

Object

# AdminAreaCriteria

The defined targeted audience by administrative area.

Search Ads 2.0+

``` source
object AdminAreaCriteria
```

## Properties

`included`

`[string]`

The dimension to include targeted users by administrative area. For example, within the United States, administrative area dimensions are states.

```
```

## Discussion

An `adminArea` is a state or the equivalent according to its associated `country`.

Use Search for Geolocations with `entity` to search for and retrieve geolocations. Then use geotargeting dimensions `country`, `adminArea`, and `locality` in the TargetingDimensions payload with the Update an Ad Group endpoint.

## See Also

### Audience Refinement

object TargetingDimensions

The optional criteria to use with ad groups to narrow the audience that views your ads.

object AppCategoryCriteria

The defined target audience by app category.

object AppDownloaderCriteria

The defined targeted audience according to app downloads.

object CountryCriteria

The defined targeted audience by country or region.

object LocalityCriteria

The defined targeted audience by locality.

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

