

- Apple Search Ads
-  DaypartCriteria 

Object

# DaypartCriteria

The defined targeted audience to include for a specific time of day.

Search Ads 2.0+

``` source
object DaypartCriteria
```

## Properties

`userTime`

DaypartDetail

The dimension to target criteria for a specific time of day. Numbers ranging from `0` to `167` represent the hours of a week beginning at Sunday 12:00 midnight. For example, the hour beginning Monday at 1:00 a.m. is `25`.

```
"daypart": {
      "userTime": {
        "included": [
          1,
          3,
          22
        ]
      }
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

object AgeRange

The defined target audience to include using the age-range demographic.

object DaypartDetail

The defined targeted audience to include by a specific time of day.

object DeviceClassCriteria

The defined targeted audience to include by device type.

object GenderCriteria

The defined targeted audience to include using the gender demographic.

