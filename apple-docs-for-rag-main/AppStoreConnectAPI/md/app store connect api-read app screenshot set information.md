

- App Store Connect API
-  Read App Screenshot Set Information 

Web Service Endpoint

# Read App Screenshot Set Information

Get an app screenshot set including its display target, language, and the screenshot it contains.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appScreenshotSets/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appScreenshotSets]`

`[string]`

Possible Values: `screenshotDisplayType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appScreenshots`

`fields[appScreenshots]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, imageAsset, assetToken, assetType, uploadOperations, assetDeliveryState, appScreenshotSet`

`include`

`[string]`

Possible Values: `appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appScreenshots`

`limit[appScreenshots]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppScreenshotSetResponse

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

