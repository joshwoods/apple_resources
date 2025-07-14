

- App Store Connect API
-  Promote a Purchase 

Web Service Endpoint

# Promote a Purchase

Add an existing in-app purchase or auto-renewable subscription to the promoted in-app purchases on an app listing in the App Store.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/promotedPurchases
```

## HTTP Body

PromotedPurchaseCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

PromotedPurchaseResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Mentioned in 

Managing auto-renewable subscriptions

Managing in-app purchases

## See Also

### Endpoints

List All Promoted Purchases for an App

Get a list of promoted in-app purchases, including promoted auto-renewable subscriptions, for an app.

List Promoted Purchase IDs for an App

Get a list of resource IDs representing promoted purchases for an auto-renewable subscription.

Read Promoted Purchase Information

Get details about a specific promoted in-app purchase.

Modify a Promoted In-App Purchase

Update the visibility of a promoted in-app purchase.

Modify the Order of a Promoted Purchase for an App

Update the order of promoted purchases.

Remove a Promoted Purchase

Remove a promotion for an in-app purchase or auto-renewable subscription from the App Store listing.

