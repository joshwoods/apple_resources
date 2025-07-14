

- App Store Connect API
-  Commit a Review Screenshot for an In-App Purchase 

Web Service Endpoint

# Commit a Review Screenshot for an In-App Purchase

Commit an uploaded image asset as a review screenshot for an in-app purchase.

App Store Connect API 2.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/inAppPurchaseAppStoreReviewScreenshots/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

InAppPurchaseAppStoreReviewScreenshotUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

InAppPurchaseAppStoreReviewScreenshotResponse

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

## Mentioned in 

Managing in-app purchases

## See Also

### Endpoints

Read In-App Purchase Review Screenshot Information

Get information about a specific review screenshot for an in-app purchase.

Create an In-App Purchase Review Screenshot

Reserve a review screenshot for an in-app purchase.

Delete a Review Screenshot for an In-App Purchase

Delete an image that you uploaded for review of an in-app purchase.

