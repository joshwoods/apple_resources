

- App Store Connect API
-  Read Game Center app version information of an App Store version 

Web Service Endpoint

# Read Game Center app version information of an App Store version

Get the status of Game Center enablement for an App Store version.

App Store Connect API 3.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/gameCenterAppVersion
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`include`

`[string]`

Possible Values: `compatibilityVersions, appStoreVersion`

`fields[gameCenterAppVersions]`

`[string]`

Possible Values: `enabled, compatibilityVersions, appStoreVersion`

`limit[compatibilityVersions]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

GameCenterAppVersionResponse

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

