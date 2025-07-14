

- App Store Connect API
-  Read in-app purchase image information 

Web Service Endpoint

# Read in-app purchase image information

Read details about a specific in-app purchase image.

App Store Connect API 3.6+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/inAppPurchaseImages/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `inAppPurchaseImages` resource ID from the List in-app purchase images response.

## HTTP Body

InAppPurchaseImageUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

InAppPurchaseImageResponse

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

Create an image for an in-app purchase

Reserve an image asset to appear in the App Store, representing an in-app purchase.

Read in-app purchase image information

Read details about a specific in-app purchase image.

List in-app purchase images

List all images for a specific in-app purchase.

Delete an in-app purchase image

Delete the image asset that appears on the App Store listing that represents an in-app purchase.

