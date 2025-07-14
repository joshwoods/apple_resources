

- App Store Connect API
-  Read Subscription Review Screenshot Information 

Web Service Endpoint

# Read Subscription Review Screenshot Information

Get the information about a review screenshot for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionAppStoreReviewScreenshots/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionAppStoreReviewScreenshots]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, imageAsset, assetToken, assetType, uploadOperations, assetDeliveryState, subscription`

`include`

`[string]`

Value: `subscription`

## Response Codes

` 200 ``OK`

SubscriptionAppStoreReviewScreenshotResponse

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

Submitting subscriptions and subscription groups for App Review

## See Also

### Endpoints

Create a Review Screenshot for an Auto-Renewable Subscription

Reserve a review screenshot for an auto-renewable subscription.

Commit a Review Screenshot for an Auto-Renewable Subscription

Commit an uploaded image asset as a review screenshot for an auto-renewable subscription.

Delete a Review Screenshot for an Auto-Renewable Subscription

Delete an image that you uploaded for review of an auto-renewable subscription.

