

- App Store Connect API
-  List the images for an in-app event 

Web Service Endpoint

# List the images for an in-app event

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appEventScreenshots/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appEventScreenshots]`

`[string]`

Possible Values: `fileSize, fileName, imageAsset, assetToken, uploadOperations, assetDeliveryState, appEventAssetType, appEventLocalization`

`include`

`[string]`

Value: `appEventLocalization`

## Response Codes

` 200 ``OK`

AppEventScreenshotResponse

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

## See Also

### Endpoints

PATCH /v1/appEventScreenshots/{id}

POST /v1/appEventScreenshots

Delete an App Event Screenshot

Delete a specific screenshot from an in-app event.

