

- App Store Connect API
-  Create an In-App Purchase Review Screenshot 

Web Service Endpoint

# Create an In-App Purchase Review Screenshot

Reserve a review screenshot for an in-app purchase.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/inAppPurchaseAppStoreReviewScreenshots
```

## HTTP Body

InAppPurchaseAppStoreReviewScreenshotCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

InAppPurchaseAppStoreReviewScreenshotResponse

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

Managing in-app purchases

## See Also

### Endpoints

Read In-App Purchase Review Screenshot Information

Get information about a specific review screenshot for an in-app purchase.

Commit a Review Screenshot for an In-App Purchase

Commit an uploaded image asset as a review screenshot for an in-app purchase.

Delete a Review Screenshot for an In-App Purchase

Delete an image that you uploaded for review of an in-app purchase.

