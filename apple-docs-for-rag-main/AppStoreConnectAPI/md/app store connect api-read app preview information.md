

- App Store Connect API
-  Read App Preview Information 

Web Service Endpoint

# Read App Preview Information

Get information about an app preview and its upload and processing status.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appPreviews/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appPreviews]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, previewFrameTimeCode, mimeType, videoUrl, previewFrameImage, previewImage, uploadOperations, assetDeliveryState, videoDeliveryState, appPreviewSet`

`include`

`[string]`

Value: `appPreviewSet`

## Response Codes

` 200 ``OK`

AppPreviewResponse

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

### Listing App Previews and Reading Information

List All App Previews for an App Preview Set

List all ordered app previews in a preview set.

