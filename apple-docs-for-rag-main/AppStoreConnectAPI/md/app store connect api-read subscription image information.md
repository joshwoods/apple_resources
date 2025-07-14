

- App Store Connect API
-  Read subscription image information 

Web Service Endpoint

# Read subscription image information

Read details about a specific subscription image.

App Store Connect API 3.6+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/subscriptionImages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `subscriptionImages` resource ID from the List subscription images response.

## HTTP Body

SubscriptionImageUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

SubscriptionImageResponse

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

## See Also

### Endpoints

Create an image for a subscription

Reserve an image asset to appear in the App Store, representing a subscription.

Read subscription image information

Read details about a specific subscription image.

List subscription images

List all images for a specific subscription.

Delete an subscription image

Delete the image asset that appears on the App Store listing that represents an subscription.

