

- App Store Connect API
-  App 

Object

# App

The data structure that represents an Apps resource.

App Store Connect API 1.0+

``` source
object App
```

## Properties

`attributes`

App.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

App.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `apps`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object App.Attributes

Attributes that describe an Apps resource.

object App.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects and data types

object AppWithoutIncludesResponse

object AppsWithoutIncludesResponse

object AppUpdateRequest

The request body you use to update an App Update.

object AppClipsResponse

A response that contains a list of App Clips resources.

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

