

- App Store Connect API
-  Read App Screenshot Information 

Web Service Endpoint

# Read App Screenshot Information

Get information about an app screenshot and its upload and processing status.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appScreenshots/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appScreenshots]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, imageAsset, assetToken, assetType, uploadOperations, assetDeliveryState, appScreenshotSet`

`include`

`[string]`

Value: `appScreenshotSet`

## Response Codes

` 200 ``OK`

AppScreenshotResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

## See Also

### Getting Screenshots and Reading Information

List All App Screenshots for an App Screenshot Set

List all ordered screenshots in a screenshot set.

