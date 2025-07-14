

- App Store Connect API
- AppInfo
-  AppInfo.Attributes 

Object

# AppInfo.Attributes

Attributes that describe an App Infos resource.

App Store Connect API 1.2+

``` source
object AppInfo.Attributes
```

## Properties

`appStoreAgeRating`

AppStoreAgeRating

The app’s age rating as it appears on the App Store for all platforms.

`appStoreState`

AppStoreVersionState

This attribute is deprecated. Use `state` instead.

`australiaAgeRating`

`string`

Possible Values: `FIFTEEN, EIGHTEEN`

`brazilAgeRating`

BrazilAgeRating

This attribute is deprecated. Use `brazilAgeRatingV2` instead.

`brazilAgeRatingV2`

`string`

The app’s age rating as it appears on the App Store in Brazil for all platforms.

Possible Values: `SELF_RATED_L, SELF_RATED_TEN, SELF_RATED_TWELVE, SELF_RATED_FOURTEEN, SELF_RATED_SIXTEEN, SELF_RATED_EIGHTEEN, OFFICIAL_L, OFFICIAL_TEN, OFFICIAL_TWELVE, OFFICIAL_FOURTEEN, OFFICIAL_SIXTEEN, OFFICIAL_EIGHTEEN`

`franceAgeRating`

`string`

Value: `EIGHTEEN`

`kidsAgeBand`

KidsAgeBand

A Made for Kids app’s age band.

`koreaAgeRating`

`string`

Possible Values: `ALL, TWELVE, FIFTEEN, NINETEEN, NOT_APPLICABLE`

`state`

`string`

Possible Values: `ACCEPTED, DEVELOPER_REJECTED, IN_REVIEW, PENDING_RELEASE, PREPARE_FOR_SUBMISSION, READY_FOR_DISTRIBUTION, READY_FOR_REVIEW, REJECTED, REPLACED_WITH_NEW_INFO, WAITING_FOR_REVIEW`

## Mentioned in 

App Store Connect API 3.3 release notes

App Store Connect API 3.7 release notes

App Store Connect API 3.8 release notes

### Discussion

Note

For more information about `australiaAgeRating` and `koreaAgeRating`, see Age Ratings in App Store Connect Help.

## See Also

### Objects

object AppInfo.Relationships

The relationships you included in the request and those on which you can operate.

