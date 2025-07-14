

- App Store Connect API
-  Read Default App Clip Experience Information 

Web Service Endpoint

# Read Default App Clip Experience Information

Get a specific default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appClipDefaultExperiences/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Default App Clip Experiences resource.

## Query Parameters

`fields[appClipAppStoreReviewDetails]`

`[string]`

Additional fields to include for each Default App Clip Experiences resource returned by the response.

Possible Values: `invocationUrls, appClipDefaultExperience`

`fields[appClipDefaultExperienceLocalizations]`

`[string]`

Additional fields to include for each Default App Clip Experiences resource returned by the response.

Possible Values: `locale, subtitle, appClipDefaultExperience, appClipHeaderImage`

`fields[appClipDefaultExperiences]`

`[string]`

Additional fields to include for each Default App Clip Experiences resource returned by the response.

Possible Values: `action, appClip, releaseWithAppStoreVersion, appClipDefaultExperienceLocalizations, appClipAppStoreReviewDetail`

`fields[appStoreVersions]`

`[string]`

Additional fields to include for each Default App Clip Experiences resource returned by the response.

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `appClip, releaseWithAppStoreVersion, appClipDefaultExperienceLocalizations, appClipAppStoreReviewDetail`

`limit[appClipDefaultExperienceLocalizations]`

`integer`

The number of included Default App Clip Experiences resources to return if the default App Clip experience localizations relationship is included.

Maximum: `50`

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

### Getting Default App Clip Experience Information

Read the App Store Review Detail for a Default App Clip Experience

Get App Store Review details for a specific default App Clip experience.

Read Localization Information for a Default App Clip Experience

Get localized metadata that appears on the App Clip card for a specific default App Clip experience.

Read App Store Version Information for a Default App Clip Experience

Get App Store Version information for a default App Clip experience.

Get the App Store Versions Resource ID for a Default App Clip Experience

Get IDs for App Store Versions related to a default App Clip experience.

