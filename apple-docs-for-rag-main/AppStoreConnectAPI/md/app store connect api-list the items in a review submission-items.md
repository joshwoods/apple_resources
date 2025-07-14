

- App Store Connect API
-  List the items in a review submission 

Web Service Endpoint

# List the items in a review submission

List all the items in a specific review submission.

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/reviewSubmissions/{id}/items
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[reviewSubmissionItems]`

`[string]`

Possible Values: `state, appStoreVersion, appCustomProductPageVersion, appStoreVersionExperiment, appStoreVersionExperimentV2, appEvent`

`limit`

`integer`

Maximum: `200`

`fields[appStoreVersionExperiments]`

`[string]`

Possible Values: `name, trafficProportion, state, reviewRequired, startDate, endDate, appStoreVersion, appStoreVersionExperimentTreatments, platform, app, latestControlVersion, controlVersions`

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[appCustomProductPageVersions]`

`[string]`

Possible Values: `version, state, deepLink, appCustomProductPage, appCustomProductPageLocalizations`

`fields[appEvents]`

`[string]`

Possible Values: `referenceName, badge, eventState, deepLink, purchaseRequirement, primaryLocale, priority, purpose, territorySchedules, archivedTerritorySchedules, localizations`

`include`

`[string]`

Possible Values: `appStoreVersion, appCustomProductPageVersion, appStoreVersionExperiment, appStoreVersionExperimentV2, appEvent`

## Response Codes

` 200 ``OK`

ReviewSubmissionItemsResponse

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

List review submissions for an app

List recent and current review submissions for a specific app.

Read review submission information

Read information about a specific review submisison.

Modify a review submission

Edit the details or contents of a review submission.

Create a review submission

Create a review submission for a specific app.

