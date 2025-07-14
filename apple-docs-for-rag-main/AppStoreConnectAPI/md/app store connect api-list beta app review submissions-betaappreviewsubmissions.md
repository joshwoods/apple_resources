

- App Store Connect API
-  List Beta App Review Submissions 

Web Service Endpoint

# List Beta App Review Submissions

Find and list beta app review submissions for all builds.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaAppReviewSubmissions
```

## Query Parameters

`fields[betaAppReviewSubmissions]`

`[string]`

Fields to return for included related types.

Possible Values: `betaReviewState, submittedDate, build`

`fields[builds]`

`[string]`

Fields to return for included related types.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`filter[betaReviewState]`

`[string]`

Attributes, relationships, and IDs by which to filter.

Possible Values: `WAITING_FOR_REVIEW, IN_REVIEW, REJECTED, APPROVED`

`filter[build]`

`[string]`

 (Required) 

Attributes, relationships, and IDs by which to filter.

`include`

`[string]`

Relationship data to include in the response.

Value: `build`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

BetaAppReviewSubmissionsResponse

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

## See Also

### Getting Beta App Review Submissions Info

Read Beta App Review Submission Information

Get a specific beta app review submission.

