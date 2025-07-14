

- App Store Connect API
-  Read the Build Information of an App Store Version 

Web Service Endpoint

# Read the Build Information of an App Store Version

Get the build that is attached to a specific App Store version.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/build
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[builds]`

`[string]`

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

## Response Codes

` 200 ``OK`

BuildWithoutIncludesResponse

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

### Attaching a Build to a Version

Get the Build ID for an App Store Version

Get the ID of the build that is attached to a specific App Store version.

Modify the Build for an App Store Version

Change the build that is attached to a specific App Store version.

