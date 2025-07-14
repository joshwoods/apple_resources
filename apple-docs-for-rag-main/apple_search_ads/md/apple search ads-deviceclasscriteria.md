

- Apple Search Ads
-  DeviceClassCriteria 

Object

# DeviceClassCriteria

The defined targeted audience to include by device type.

Search Ads 2.0+

``` source
object DeviceClassCriteria
```

## Properties

`included`

`[string]`

The dimension to include the targeting criteria values for device class targeting.

This parameter doesn’t support the `excluded` attribute.

```
"deviceClass": {
      "included": [
        "IPAD",
        "IPHONE"
      ]
    },
```

Possible Values: `IPAD, IPHONE`

## Discussion

If you don’t set the `DeviceClassCriteria`, the API targets the currently supported devices by default.

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

object DaypartCriteria

The defined targeted audience to include for a specific time of day.

object DaypartDetail

The defined targeted audience to include by a specific time of day.

object GenderCriteria

The defined targeted audience to include using the gender demographic.

