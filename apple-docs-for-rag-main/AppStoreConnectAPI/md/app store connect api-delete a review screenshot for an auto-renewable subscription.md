

- App Store Connect API
-  Delete a Review Screenshot for an Auto-Renewable Subscription 

Web Service Endpoint

# Delete a Review Screenshot for an Auto-Renewable Subscription

Delete an image that you uploaded for review of an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/subscriptionAppStoreReviewScreenshots/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

## See Also

### Endpoints

Read Subscription Review Screenshot Information

Get the information about a review screenshot for an auto-renewable subscription.

Create a Review Screenshot for an Auto-Renewable Subscription

Reserve a review screenshot for an auto-renewable subscription.

Commit a Review Screenshot for an Auto-Renewable Subscription

Commit an uploaded image asset as a review screenshot for an auto-renewable subscription.

