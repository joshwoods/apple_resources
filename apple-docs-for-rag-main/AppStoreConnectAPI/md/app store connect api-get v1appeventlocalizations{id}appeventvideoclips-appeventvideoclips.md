

- App Store Connect API
-  GET /v1/appEventLocalizations/{id}/appEventVideoClips 

Web Service Endpoint

# GET /v1/appEventLocalizations/{id}/appEventVideoClips

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appEventLocalizations/{id}/appEventVideoClips
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appEventVideoClips]`

`[string]`

Possible Values: `fileSize, fileName, previewFrameTimeCode, videoUrl, previewFrameImage, previewImage, uploadOperations, assetDeliveryState, videoDeliveryState, appEventAssetType, appEventLocalization`

`limit`

`integer`

Maximum: `200`

`fields[appEventLocalizations]`

`[string]`

Possible Values: `locale, name, shortDescription, longDescription, appEvent, appEventScreenshots, appEventVideoClips`

`include`

`[string]`

Value: `appEventLocalization`

## Response Codes

` 200 ``OK`

AppEventVideoClipsResponse

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

GET /v1/appEventLocalizations/{id}

GET /v1/appEventLocalizations/{id}/appEventScreenshots

PATCH /v1/appEventLocalizations/{id}

POST /v1/appEventLocalizations

Delete an App Event Localization

Delete localized metadata that you configured for an in-app event.

