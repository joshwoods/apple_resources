

- App Store Connect API
-  List app preview sets for a custom product page localization 

Web Service Endpoint

# List app preview sets for a custom product page localization

List the app preview sets for a specific custom product page localization.

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appCustomProductPageLocalizations/{id}/appPreviewSets
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app custom product page localization resource ID from the List custom product pages localizations response.

## Query Parameters

`fields[appPreviewSets]`

`[string]`

Possible Values: `previewType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appPreviews`

`fields[appPreviews]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, previewFrameTimeCode, mimeType, videoUrl, previewFrameImage, previewImage, uploadOperations, assetDeliveryState, videoDeliveryState, appPreviewSet`

`filter[appStoreVersionExperimentTreatmentLocalization]`

`[string]`

`filter[appStoreVersionLocalization]`

`[string]`

`filter[previewType]`

`[string]`

Possible Values: `IPHONE_67, IPHONE_61, IPHONE_65, IPHONE_58, IPHONE_55, IPHONE_47, IPHONE_40, IPHONE_35, IPAD_PRO_3GEN_129, IPAD_PRO_3GEN_11, IPAD_PRO_129, IPAD_105, IPAD_97, DESKTOP, APPLE_TV, APPLE_VISION_PRO`

`include`

`[string]`

Possible Values: `appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appPreviews`

`limit`

`integer`

Maximum: `200`

`limit[appPreviews]`

`integer`

Maximum: `50`

`fields[appCustomProductPageLocalizations]`

`[string]`

Possible Values: `locale, promotionalText, appCustomProductPageVersion, appScreenshotSets, appPreviewSets`

`fields[appStoreVersionExperimentTreatmentLocalizations]`

`[string]`

Possible Values: `locale, appStoreVersionExperimentTreatment, appScreenshotSets, appPreviewSets`

`fields[appStoreVersionLocalizations]`

`[string]`

Possible Values: `description, locale, keywords, marketingUrl, promotionalText, supportUrl, whatsNew, appStoreVersion, appScreenshotSets, appPreviewSets`

## Response Codes

` 200 ``OK`

AppPreviewSetsResponse

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

Create an App Preview Set

Add a new app preview set to an App Store version localization for a specific app preview type and display size.

Delete an App Preview Set

Delete an app preview set and all of its previews.

List All App Previews for an App Preview Set

List all ordered app previews in a preview set.

Get All App Preview IDs for an App Preview Set

Get the ordered app preview IDs in a preview set.

Replace All App Previews for an App Preview Set

Change the order of the app previews in a preview set.

