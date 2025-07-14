

- App Store Connect API
-  Read Build Beta Detail Information 

Web Service Endpoint

# Read Build Beta Detail Information

Get a specific build beta details resource.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/buildBetaDetails/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`fields[buildBetaDetails]`

`[string]`

Fields to return for included related types.

Possible Values: `autoNotifyEnabled, internalBuildState, externalBuildState, build`

`fields[builds]`

`[string]`

Fields to return for included related types.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`include`

`[string]`

Relationship data to include in the response.

Value: `build`

## Response Codes

` 200 ``OK`

BuildBetaDetailResponse

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

### Getting Build Beta Details Information

List Build Beta Details

Find and list build beta details for all builds.

Read the Build Information of a Build Beta Detail

Get the build information for a specific build beta details resource.

