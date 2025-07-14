

- Apple Search Ads
-  AgeRange 

Object

# AgeRange

The defined target audience to include using the age-range demographic.

Search Ads 2.0+

``` source
object AgeRange
```

## Properties

`maxAge`

`int32`

The dimension for specifying the maximum age for targeting. This field may be `null`.

Maximum: `65`

`minAge`

`int32`

The dimension for specifying the minimum age for targeting. The minimum value is `18`.

Maximum: `65`

## Discussion

Use this dimension to limit the age group to target your ad to.

```
    "age": {
      "included": [
        {
          "minAge": 20,
          "maxAge": 25
        }

```

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

object LocalityCriteria

The defined targeted audience by locality.

object AgeCriteria

The defined targeted audience to include using the age demographic.

object DaypartCriteria

The defined targeted audience to include for a specific time of day.

object DaypartDetail

The defined targeted audience to include by a specific time of day.

object DeviceClassCriteria

The defined targeted audience to include by device type.

object GenderCriteria

The defined targeted audience to include using the gender demographic.

