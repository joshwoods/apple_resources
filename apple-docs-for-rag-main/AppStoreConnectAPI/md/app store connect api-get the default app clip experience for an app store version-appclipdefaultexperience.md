

- App Store Connect API
-  Get the Default App Clip Experience for an App Store Version 

Web Service Endpoint

# Get the Default App Clip Experience for an App Store Version

Get the default App Clip experience for an App Store version of your app.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/appClipDefaultExperience
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the App Store Versions resource.

## Query Parameters

`fields[appClipDefaultExperienceLocalizations]`

`[string]`

Additional fields to include for each Default App Clip Experiences resource returned by the response.

Possible Values: `locale, subtitle, appClipDefaultExperience, appClipHeaderImage`

`fields[appClipDefaultExperiences]`

`[string]`

Additional fields to include for each Default App Clip Experiences resource returned by the response.

Possible Values: `action, appClip, releaseWithAppStoreVersion, appClipDefaultExperienceLocalizations, appClipAppStoreReviewDetail`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `appClip, releaseWithAppStoreVersion, appClipDefaultExperienceLocalizations, appClipAppStoreReviewDetail`

`limit[appClipDefaultExperienceLocalizations]`

`integer`

The number of included Default App Clip Experiences resources to return if the default App Clip experience localizations relationship is included.

Maximum: `50`

`fields[appClips]`

`[string]`

Possible Values: `bundleId, app, appClipDefaultExperiences, appClipAdvancedExperiences`

`fields[appClipAppStoreReviewDetails]`

`[string]`

Possible Values: `invocationUrls, appClipDefaultExperience`

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

## Response Codes

` 200 ``OK`

AppClipDefaultExperienceResponse

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

### Attaching a Default App Clip Experience to a Version

Get the Default App Clip Experiences Resource ID for an App Store Version

Get the ID of an app’s related default App Clip experience.

Modify the Default App Clip Experience of an App Store Version

Update the relationship between an App Store version and a default App Clip experience.

