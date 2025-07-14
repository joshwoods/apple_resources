

- App Store Connect API
-  Modify an In-App Purchase Localization 

Web Service Endpoint

# Modify an In-App Purchase Localization

Update the display name and description for a specific locale of an in-app purchase.

App Store Connect API 2.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/inAppPurchaseLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

InAppPurchaseLocalizationUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

InAppPurchaseLocalizationResponse

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

Note

Changes that you make to product metadata with the App Store Connect API can take up to 1 hour to appear in the sandbox environment.

## See Also

### Endpoints

List All Localizations for an In-App Purchase

Get a list of localized display names and descriptions for a specific in-app purchase.

Create an In-App Purchase Localization

Create a localized display name and description for an in-app purchase.

Read In-App Purchase Localization Information

Get the display name and description for a specific locale for an in-app purchase.

Delete an In-App Purchase Localization

Delete the metadata for a single in-app purchase localization.

