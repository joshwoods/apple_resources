

- App Store Connect API
-  AppClipsResponse 

Object

# AppClipsResponse

A response that contains a list of App Clips resources.

App Store Connect API 1.6+

``` source
object AppClipsResponse
```

## Properties

`data`

`[`AppClip`]`

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: App`, `AppClipDefaultExperience

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## See Also

### Objects and data types

object App

The data structure that represents an Apps resource.

object AppWithoutIncludesResponse

object AppsWithoutIncludesResponse

object AppUpdateRequest

The request body you use to update an App Update.

object AppResponse

A response that contains a single Apps resource.

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

