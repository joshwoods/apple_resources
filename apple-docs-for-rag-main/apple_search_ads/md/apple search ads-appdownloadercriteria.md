

- Apple Search Ads
-  AppDownloaderCriteria 

Object

# AppDownloaderCriteria

The defined targeted audience according to app downloads.

Search Ads 2.0+

``` source
object AppDownloaderCriteria
```

## Properties

`excluded`

`[string]`

The dimension to limit viewing of your ad to users who have not downloaded your app.

```
{
  "appDownloaders": {
    "excluded": 654327167
  }
}
```

`included`

`[string]`

The dimension to limit viewing of your ad to users who have downloaded your app.

```
{
  "appDownloaders": {
    "included": 654327143

  }
}
```

## Discussion

To target all users, don’t include the `AppDownloaderCriteria` dimension in the request payload.

Use the `adamId` of the app you’re promoting in your campaign as an `included` or `excluded` value. You can obtain your app `adamId` through Get a Campaign, Get all Campaigns, or Search for iOS apps using the `returnOwnedApps` query.

## See Also

### Audience Refinement

object TargetingDimensions

The optional criteria to use with ad groups to narrow the audience that views your ads.

object AppCategoryCriteria

The defined target audience by app category.

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

