

- App Store Connect API
-  List All Localizations for an In-App Purchase 

Web Service Endpoint

# List All Localizations for an In-App Purchase

Get a list of localized display names and descriptions for a specific in-app purchase.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v2/inAppPurchases/{id}/inAppPurchaseLocalizations
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[inAppPurchaseLocalizations]`

`[string]`

Possible Values: `name, locale, description, state, inAppPurchaseV2`

`fields[inAppPurchases]`

`[string]`

Possible Values: `name, productId, inAppPurchaseType, state, reviewNote, familySharable, contentHosting, inAppPurchaseLocalizations, pricePoints, content, appStoreReviewScreenshot, promotedPurchase, iapPriceSchedule, inAppPurchaseAvailability, images`

`include`

`[string]`

Value: `inAppPurchaseV2`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

InAppPurchaseLocalizationsResponse

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

## Mentioned in 

Managing in-app purchases

## See Also

### Endpoints

Create an In-App Purchase Localization

Create a localized display name and description for an in-app purchase.

Read In-App Purchase Localization Information

Get the display name and description for a specific locale for an in-app purchase.

Modify an In-App Purchase Localization

Update the display name and description for a specific locale of an in-app purchase.

Delete an In-App Purchase Localization

Delete the metadata for a single in-app purchase localization.

