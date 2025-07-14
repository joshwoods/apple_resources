

- App Store Connect API
-  GET /v1/appEventLocalizations/{id} 

Web Service Endpoint

# GET /v1/appEventLocalizations/{id}

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appEventLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appEventLocalizations]`

`[string]`

Possible Values: `locale, name, shortDescription, longDescription, appEvent, appEventScreenshots, appEventVideoClips`

`fields[appEventScreenshots]`

`[string]`

Possible Values: `fileSize, fileName, imageAsset, assetToken, uploadOperations, assetDeliveryState, appEventAssetType, appEventLocalization`

`fields[appEventVideoClips]`

`[string]`

Possible Values: `fileSize, fileName, previewFrameTimeCode, videoUrl, previewFrameImage, previewImage, uploadOperations, assetDeliveryState, videoDeliveryState, appEventAssetType, appEventLocalization`

`include`

`[string]`

Possible Values: `appEvent, appEventScreenshots, appEventVideoClips`

`limit[appEventScreenshots]`

`integer`

Maximum: `50`

`limit[appEventVideoClips]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppEventLocalizationResponse

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

GET /v1/appEventLocalizations/{id}/appEventVideoClips

GET /v1/appEventLocalizations/{id}/appEventScreenshots

PATCH /v1/appEventLocalizations/{id}

POST /v1/appEventLocalizations

Delete an App Event Localization

Delete localized metadata that you configured for an in-app event.

