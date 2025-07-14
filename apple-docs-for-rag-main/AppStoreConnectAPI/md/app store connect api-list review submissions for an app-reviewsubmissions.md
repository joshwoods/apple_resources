

- App Store Connect API
-  List review submissions for an app 

Web Service Endpoint

# List review submissions for an app

List recent and current review submissions for a specific app.

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/reviewSubmissions
```

## Query Parameters

`fields[reviewSubmissionItems]`

`[string]`

Possible Values: `state, appStoreVersion, appCustomProductPageVersion, appStoreVersionExperiment, appStoreVersionExperimentV2, appEvent`

`fields[reviewSubmissions]`

`[string]`

Possible Values: `platform, submittedDate, state, app, items, appStoreVersionForReview, submittedByActor, lastUpdatedByActor`

`filter[app]`

`[string]`

 (Required) 

`filter[platform]`

`[string]`

Possible Values: `IOS, MAC_OS, TV_OS, VISION_OS`

`filter[state]`

`[string]`

Possible Values: `READY_FOR_REVIEW, WAITING_FOR_REVIEW, IN_REVIEW, UNRESOLVED_ISSUES, CANCELING, COMPLETING, COMPLETE`

`include`

`[string]`

Possible Values: `app, items, appStoreVersionForReview, submittedByActor, lastUpdatedByActor`

`limit`

`integer`

Maximum: `200`

`limit[items]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

ReviewSubmissionsResponse

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

## See Also

### Endpoints

Read review submission information

Read information about a specific review submisison.

List the items in a review submission

List all the items in a specific review submission.

Modify a review submission

Edit the details or contents of a review submission.

Create a review submission

Create a review submission for a specific app.

