

- App Store Connect API
-  Read App Clip Information 

Web Service Endpoint

# Read App Clip Information

Get a specific App Clip.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appClips/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the App Clips resource.

## Query Parameters

`fields[appClipDefaultExperiences]`

`[string]`

Additional fields to include for each App Clips resource returned by the response.

Possible Values: `action, appClip, releaseWithAppStoreVersion, appClipDefaultExperienceLocalizations, appClipAppStoreReviewDetail`

`fields[appClips]`

`[string]`

Additional fields to include for each App Clips resource returned by the response.

Possible Values: `bundleId, app, appClipDefaultExperiences, appClipAdvancedExperiences`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `app, appClipDefaultExperiences`

`limit[appClipDefaultExperiences]`

`integer`

The number of included App Clips resources to return if the default App Clip experience localizations relationship is included.

Maximum: `50`

## Response Codes

` 200 ``OK`

AppClipResponse

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

