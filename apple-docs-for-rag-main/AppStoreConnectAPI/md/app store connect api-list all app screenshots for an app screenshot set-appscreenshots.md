

- App Store Connect API
-  List All App Screenshots for an App Screenshot Set 

Web Service Endpoint

# List All App Screenshots for an App Screenshot Set

List all ordered screenshots in a screenshot set.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appScreenshotSets/{id}/appScreenshots
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appScreenshots]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, imageAsset, assetToken, assetType, uploadOperations, assetDeliveryState, appScreenshotSet`

`limit`

`integer`

Maximum: `200`

`fields[appScreenshotSets]`

`[string]`

Possible Values: `screenshotDisplayType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appScreenshots`

`include`

`[string]`

Value: `appScreenshotSet`

## Response Codes

` 200 ``OK`

AppScreenshotsResponse

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

### Listing and Reordering All Screenshots in a Set

Get All App Screenshot IDs for an App Screenshot Set

Get the ordered screenshot IDs in a screenshot set.

Replace All App Screenshots for an App Screenshot Set

Change the order of the screenshots in a screenshot set.

