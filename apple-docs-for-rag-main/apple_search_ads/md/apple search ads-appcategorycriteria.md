

- Apple Search Ads
-  AppCategoryCriteria 

Object

# AppCategoryCriteria

The defined target audience by app category.

Search Ads 4.6+

``` source
object AppCategoryCriteria
```

## Properties

`excluded`

`[integer]`

A value of `100` indicates that you aren’t targeting apps with the same app category as your app.

`included`

`[integer]`

A value of `100` indicates that you are targeting apps with the same app category as your app.

## Mentioned in 

Apple Search Ads Campaign Management API 4

## Discussion

The app category targeting dimension is optional and is only applicable to campaigns using a SupplySource of `APPSTORE_PRODUCT_PAGES_BROWSE`. See the App Store for more details about categories.

## See Also

### Audience Refinement

object TargetingDimensions

The optional criteria to use with ad groups to narrow the audience that views your ads.

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

object DeviceClassCriteria

The defined targeted audience to include by device type.

object GenderCriteria

The defined targeted audience to include using the gender demographic.

