

- Apple Search Ads
-  AgeCriteria 

Object

# AgeCriteria

The defined targeted audience to include using the age demographic.

Search Ads 2.0+

``` source
object AgeCriteria
```

## Properties

`included`

`[`AgeRange`]`

The dimension to include age-range targeting criteria.

```
"age": {
      "included": [
        {
          "minAge": 20,
          "maxAge": 25
        }
      ]
    },
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

