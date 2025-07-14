

- App Store Connect API
-  Read an App’s Encryption Declarations 

Web Service Endpoint

# Read an App’s Encryption Declarations

Find and list all available app encryption declarations.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/appEncryptionDeclarations
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appEncryptionDeclarationDocuments]`

`[string]`

Possible Values: `fileSize, fileName, assetToken, downloadUrl, sourceFileChecksum, uploadOperations, assetDeliveryState`

`fields[appEncryptionDeclarations]`

`[string]`

Possible Values: `appDescription, createdDate, usesEncryption, exempt, containsProprietaryCryptography, containsThirdPartyCryptography, availableOnFrenchStore, platform, uploadedDate, documentUrl, documentName, documentType, appEncryptionDeclarationState, codeValue, app, builds, appEncryptionDeclarationDocument`

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[builds]`

`[string]`

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`filter[builds]`

`[string]`

`filter[platform]`

`[string]`

Deprecated 

Possible Values: `IOS, MAC_OS, TV_OS, VISION_OS`

`include`

`[string]`

Possible Values: `app, builds, appEncryptionDeclarationDocument`

`limit`

`integer`

Maximum: `200`

`limit[builds]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppEncryptionDeclarationsResponse

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

App Store Connect API 3.0 release notes

## See Also

### Getting and modifying app information

List Apps

Find and list apps in App Store Connect.

Read App Information

Get information about a specific app.

Modify an App

Update app information, including bundle ID, primary locale, price schedule, and global availability.

