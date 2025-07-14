

- Apple Search Ads
-  CountryCriteria 

Object

# CountryCriteria

The defined targeted audience by country or region.

Search Ads 2.0+

``` source
object CountryCriteria
```

## Properties

`included`

`[string]`

The dimension to include targeted users by country or region.

Note

For reports, `countryCriteria` must be the same location as the specified CountryOrRegion.

## Discussion

Use Search for Geolocations with `entity` to search for and retrieve geolocations. Then use geotargeting dimensions `country`, `adminArea`, and `locality` in the TargetingDimensions payload with Create an Ad Group and Update an Ad Group endpoints. For the country dimension, use two-letter country codes in ISO 3166-1 alpha-2 country code format. Campaigns that serve multiple countries or regions can’t use geotargeting. Use UpdateCampaignRequest to clear geotargeting from a campaign.

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

