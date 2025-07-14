

- App Store Connect API
-  List Beta Build Localizations 

Web Service Endpoint

# List Beta Build Localizations

Find and list beta build localizations currently associated with apps.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaBuildLocalizations
```

## Query Parameters

`fields[betaBuildLocalizations]`

`[string]`

Fields to return for included related types.

Possible Values: `whatsNew, locale, build`

`fields[builds]`

`[string]`

Fields to return for included related types.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`filter[build]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[locale]`

`[string]`

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

BetaBuildLocalizationsResponse

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

### Getting Build Information

Read Beta Build Localization Information

Get a specific beta build localization resource.

Read the Build Information of a Beta Build Localization

Get the build information for a specific beta build localization.

