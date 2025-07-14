

- App Store Connect API
-  Read the Beta App Review Submission of a Build 

Web Service Endpoint

# Read the Beta App Review Submission of a Build

Get the beta app review submission status for a specific build.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/builds/{id}/betaAppReviewSubmission
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`fields[betaAppReviewSubmissions]`

`[string]`

Fields to return for included related types.

Possible Values: `betaReviewState, submittedDate, build`

## Response Codes

` 200 ``OK`

BetaAppReviewSubmissionWithoutIncludesResponse

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

