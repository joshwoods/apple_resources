

- App Store Connect API
-  Read review submission information 

Web Service Endpoint

# Read review submission information

Read information about a specific review submisison.

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/reviewSubmissions/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[reviewSubmissionItems]`

`[string]`

Possible Values: `state, appStoreVersion, appCustomProductPageVersion, appStoreVersionExperiment, appStoreVersionExperimentV2, appEvent`

`fields[reviewSubmissions]`

`[string]`

Possible Values: `platform, submittedDate, state, app, items, appStoreVersionForReview, submittedByActor, lastUpdatedByActor`

`include`

`[string]`

Possible Values: `app, items, appStoreVersionForReview, submittedByActor, lastUpdatedByActor`

`limit[items]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

ReviewSubmissionResponse

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

List the items in a review submission

List all the items in a specific review submission.

Modify a review submission

Edit the details or contents of a review submission.

Create a review submission

Create a review submission for a specific app.

