

- App Store Connect API
-  GET /v1/appEvents/{id}/localizations 

Web Service Endpoint

# GET /v1/appEvents/{id}/localizations

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appEvents/{id}/localizations
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

`limit`

`integer`

Maximum: `200`

`limit[appEventScreenshots]`

`integer`

Maximum: `50`

`limit[appEventVideoClips]`

`integer`

Maximum: `50`

`fields[appEvents]`

`[string]`

Possible Values: `referenceName, badge, eventState, deepLink, purchaseRequirement, primaryLocale, priority, purpose, territorySchedules, archivedTerritorySchedules, localizations`

## Response Codes

` 200 ``OK`

AppEventLocalizationsResponse

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

Read in-app event information

GET /v1/apps/{id}/appEvents

PATCH /v1/appEvents/{id}

POST /v1/appEvents

Delete an App Event

Delete an in-app event and its related metadata.

