

- App Store Connect API
-  AppResponse 

Object

# AppResponse

A response that contains a single Apps resource.

App Store Connect API 1.0+

``` source
object AppResponse
```

## Properties

`data`

App

 (Required) 

The resource data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

`included`

`[*]`

Possible types: AppEncryptionDeclaration`, `CiProduct`, `BetaGroup`, `AppStoreVersion`, `PrereleaseVersion`, `BetaAppLocalization`, `Build`, `BetaLicenseAgreement`, `BetaAppReviewDetail`, `AppInfo`, `AppClip`, `EndUserLicenseAgreement`, `InAppPurchase`, `SubscriptionGroup`, `GameCenterEnabledVersion`, `AppCustomProductPage`, `InAppPurchaseV2`, `PromotedPurchase`, `AppEvent`, `ReviewSubmission`, `SubscriptionGracePeriod`, `GameCenterDetail`, `AppStoreVersionExperimentV2

## See Also

### Related Documentation

Read the App Information of an App Encryption Declaration

Get the app information from a specific app encryption declaration.

Deprecated

### Objects and data types

object App

The data structure that represents an Apps resource.

object AppWithoutIncludesResponse

object AppsWithoutIncludesResponse

object AppUpdateRequest

The request body you use to update an App Update.

object AppClipsResponse

A response that contains a list of App Clips resources.

object AppsResponse

A response that contains a list of Apps resources.

object InAppPurchase

The data structure that represents the In-App Purchases resource.

Deprecated

object InAppPurchaseResponse

A response that contains a single In-App Purchases resource.

Deprecated

object InAppPurchasesResponse

A response that contains a list of In-App Purchases resources.

Deprecated

object AppBetaTestersLinkagesRequest

A request body you use to remove beta testers from an app.

object AppPricePointV3

The data structure that represents an App Price Point V3 resource.

object AppPricePointV3Response

object AppPricePointsV3Response

object AppPriceSchedule

object AppPriceScheduleCreateRequest

