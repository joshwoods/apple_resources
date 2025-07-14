

- App Store Connect API
-  Submit an App for Beta Review 

Web Service Endpoint

# Submit an App for Beta Review

Submit an app for beta app review to allow external testing.

App Store Connect API 1.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/betaAppReviewSubmissions
```

## HTTP Body

BetaAppReviewSubmissionCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

BetaAppReviewSubmissionResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Overview

Important

Before submitting to beta app review, you need to add a description for all `betaAppLocalizations`. To add a description, use Modify a Beta App Localization.

