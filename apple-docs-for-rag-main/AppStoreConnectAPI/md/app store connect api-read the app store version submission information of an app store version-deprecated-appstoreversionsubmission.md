

- App Store Connect API
-  Read the App Store Version Submission Information of an App Store Version Deprecated

Web Service Endpoint

# Read the App Store Version Submission Information of an App Store Version

App Store Connect API 1.2–1.7Deprecated

Deprecated

Use Read review submission information instead.

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/appStoreVersionSubmission
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appStoreVersionSubmissions]`

`[string]`

Value: `appStoreVersion`

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`include`

`[string]`

Value: `appStoreVersion`

## Response Codes

` 200 ``OK`

AppStoreVersionSubmissionResponse

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

### Reading Release and Review Information

Read the App Store Review Details Resource Information of an App Store Version

Get the details you provide to App Review so they can test your app.

Read the App Store Version Phased Release Information of an App Store Version

Read the phased release status and configuration for a version with phased release enabled.

