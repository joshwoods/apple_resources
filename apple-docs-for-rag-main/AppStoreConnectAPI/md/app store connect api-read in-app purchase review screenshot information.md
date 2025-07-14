

- App Store Connect API
-  Read In-App Purchase Review Screenshot Information 

Web Service Endpoint

# Read In-App Purchase Review Screenshot Information

Get information about a specific review screenshot for an in-app purchase.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/inAppPurchaseAppStoreReviewScreenshots/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[inAppPurchaseAppStoreReviewScreenshots]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, imageAsset, assetToken, assetType, uploadOperations, assetDeliveryState, inAppPurchaseV2`

`include`

`[string]`

Value: `inAppPurchaseV2`

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

## Mentioned in 

Managing in-app purchases

## See Also

### Endpoints

Create an In-App Purchase Review Screenshot

Reserve a review screenshot for an in-app purchase.

Commit a Review Screenshot for an In-App Purchase

Commit an uploaded image asset as a review screenshot for an in-app purchase.

Delete a Review Screenshot for an In-App Purchase

Delete an image that you uploaded for review of an in-app purchase.

