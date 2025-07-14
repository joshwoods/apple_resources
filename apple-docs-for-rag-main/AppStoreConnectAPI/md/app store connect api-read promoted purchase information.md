

- App Store Connect API
-  Read Promoted Purchase Information 

Web Service Endpoint

# Read Promoted Purchase Information

Get details about a specific promoted in-app purchase.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/promotedPurchases/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[promotedPurchases]`

`[string]`

Possible Values: `visibleForAllUsers, enabled, state, inAppPurchaseV2, subscription`

`include`

`[string]`

Possible Values: `inAppPurchaseV2, subscription`

## Response Codes

` 200 ``OK`

PromotedPurchaseResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## See Also

### Endpoints

Promote a Purchase

Add an existing in-app purchase or auto-renewable subscription to the promoted in-app purchases on an app listing in the App Store.

List All Promoted Purchases for an App

Get a list of promoted in-app purchases, including promoted auto-renewable subscriptions, for an app.

List Promoted Purchase IDs for an App

Get a list of resource IDs representing promoted purchases for an auto-renewable subscription.

Modify a Promoted In-App Purchase

Update the visibility of a promoted in-app purchase.

Modify the Order of a Promoted Purchase for an App

Update the order of promoted purchases.

Remove a Promoted Purchase

Remove a promotion for an in-app purchase or auto-renewable subscription from the App Store listing.

