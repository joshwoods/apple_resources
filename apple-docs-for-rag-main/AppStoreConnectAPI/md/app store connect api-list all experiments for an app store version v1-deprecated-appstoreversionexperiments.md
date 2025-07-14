

- App Store Connect API
-  List All Experiments for an App Store Version v1 Deprecated

Web Service Endpoint

# List All Experiments for an App Store Version v1

Get a list of all experiments for an App Store version of an app across all platforms.

App Store Connect API 1.7–2.4Deprecated

Deprecated

Use List All Experiments for an App Store Version instead.

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/appStoreVersionExperiments
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List All App Store Versions for an App response.

## Query Parameters

`fields[appStoreVersionExperimentTreatments]`

`[string]`

Possible Values: `name, appIcon, appIconName, promotedDate, appStoreVersionExperiment, appStoreVersionExperimentV2, appStoreVersionExperimentTreatmentLocalizations`

`fields[appStoreVersionExperiments]`

`[string]`

Possible Values: `name, trafficProportion, state, reviewRequired, startDate, endDate, appStoreVersion, appStoreVersionExperimentTreatments`

`filter[state]`

`[string]`

Possible Values: `PREPARE_FOR_SUBMISSION, READY_FOR_REVIEW, WAITING_FOR_REVIEW, IN_REVIEW, ACCEPTED, APPROVED, REJECTED, COMPLETED, STOPPED`

`include`

`[string]`

Possible Values: `appStoreVersion, appStoreVersionExperimentTreatments`

`limit`

`integer`

Maximum: `200`

`limit[appStoreVersionExperimentTreatments]`

`integer`

Maximum: `50`

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

## Response Codes

` 200 ``OK`

AppStoreVersionExperimentsResponse

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

## Mentioned in 

App Store Connect API 2.4 release notes

## See Also

### Getting App Store Version Experiments

List All Experiments for an App Store Version

Get a list of all experiments for an App Store version of an app across all platforms.

