

- App Store Connect API
-  Create a Review Screenshot for an Auto-Renewable Subscription 

Web Service Endpoint

# Create a Review Screenshot for an Auto-Renewable Subscription

Reserve a review screenshot for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/subscriptionAppStoreReviewScreenshots
```

## HTTP Body

SubscriptionAppStoreReviewScreenshotCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

SubscriptionAppStoreReviewScreenshotResponse

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

Submitting subscriptions and subscription groups for App Review

## See Also

### Endpoints

Read Subscription Review Screenshot Information

Get the information about a review screenshot for an auto-renewable subscription.

Commit a Review Screenshot for an Auto-Renewable Subscription

Commit an uploaded image asset as a review screenshot for an auto-renewable subscription.

Delete a Review Screenshot for an Auto-Renewable Subscription

Delete an image that you uploaded for review of an auto-renewable subscription.

