

- App Store Connect API
-  List All Advanced App Clip Experiences for an App Clip 

Web Service Endpoint

# List All Advanced App Clip Experiences for an App Clip

Get all advanced App Clip experiences for an App Clip.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appClips/{id}/appClipAdvancedExperiences
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the App Clips resource.

## Query Parameters

`fields[appClipAdvancedExperienceLocalizations]`

`[string]`

Additional fields to include for each Advanced App Clip Experiences resource returned by the response.

Possible Values: `language, title, subtitle`

`fields[appClipAdvancedExperiences]`

`[string]`

Additional fields to include for each Advanced App Clip Experiences resource returned by the response.

Possible Values: `link, version, status, action, isPoweredBy, place, placeStatus, businessCategory, defaultLanguage, appClip, headerImage, localizations`

`filter[action]`

`[string]`

Filter the returned advanced App Clip experiences using the verb that appears on the App Clip card.

Possible Values: `OPEN, VIEW, PLAY`

`filter[placeStatus]`

`[string]`

Filter the returned advanced App Clip experiences using the status of the associated place in Apple Maps.

Possible Values: `PENDING, MATCHED, NO_MATCH`

`filter[status]`

`[string]`

Filter the returned advanced App Clip experiences using their status.

Possible Values: `RECEIVED, DEACTIVATED, APP_TRANSFER_IN_PROGRESS`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `appClip, headerImage, localizations`

`limit`

`integer`

The number of Advanced App Clip Experiences resources to return.

Maximum: `200`

`limit[localizations]`

`integer`

The number of included Advanced App Clip Experiences resources to return if the advanced App Clip experience localizations relationship is included.

Maximum: `50`

`fields[appClips]`

`[string]`

Possible Values: `bundleId, app, appClipDefaultExperiences, appClipAdvancedExperiences`

`fields[appClipAdvancedExperienceImages]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, imageAsset, uploadOperations, assetDeliveryState`

## Response Codes

` 200 ``OK`

AppClipAdvancedExperiencesResponse

`OK`

The request completed successfully.

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

### Getting App Clip Experiences

List All Default App Clip Experiences for an App Clip

Get all default App Clip experiences for an App Clip.

