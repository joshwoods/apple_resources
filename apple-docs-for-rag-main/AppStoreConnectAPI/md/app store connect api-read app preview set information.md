

- App Store Connect API
-  Read App Preview Set Information 

Web Service Endpoint

# Read App Preview Set Information

Get an app preview set that includes its display target, language, and the previews it contains.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appPreviewSets/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appPreviewSets]`

`[string]`

Possible Values: `previewType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appPreviews`

`fields[appPreviews]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, previewFrameTimeCode, mimeType, videoUrl, previewFrameImage, previewImage, uploadOperations, assetDeliveryState, videoDeliveryState, appPreviewSet`

`include`

`[string]`

Possible Values: `appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appPreviews`

`limit[appPreviews]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppPreviewSetResponse

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

