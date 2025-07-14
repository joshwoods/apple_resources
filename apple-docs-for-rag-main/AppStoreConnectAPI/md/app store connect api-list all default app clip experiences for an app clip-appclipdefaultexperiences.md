

- App Store Connect API
-  List All Default App Clip Experiences for an App Clip 

Web Service Endpoint

# List All Default App Clip Experiences for an App Clip

Get all default App Clip experiences for an App Clip.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appClips/{id}/appClipDefaultExperiences
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the App Clips resource.

## Query Parameters

`exists[releaseWithAppStoreVersion]`

`boolean`

Only include Default App Clip Experiences resources that have a related App Store Versions resource.

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

`limit`

`integer`

The number of Default App Clip Experiences resources to return.

Maximum: `200`

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

AppClipDefaultExperiencesResponse

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

List All Advanced App Clip Experiences for an App Clip

Get all advanced App Clip experiences for an App Clip.

