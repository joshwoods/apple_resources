

- App Store Connect API
-  List Builds 

Web Service Endpoint

# List Builds

Find and list builds for all apps in App Store Connect.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/builds
```

## Query Parameters

`fields[appEncryptionDeclarations]`

`[string]`

Fields to return for included related types.

Possible Values: `appDescription, createdDate, usesEncryption, exempt, containsProprietaryCryptography, containsThirdPartyCryptography, availableOnFrenchStore, platform, uploadedDate, documentUrl, documentName, documentType, appEncryptionDeclarationState, codeValue, app, builds, appEncryptionDeclarationDocument`

`fields[apps]`

`[string]`

Fields to return for included related types.

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[betaTesters]`

`[string]`

Fields to return for included related types.

Possible Values: `firstName, lastName, email, inviteType, state, apps, betaGroups, builds`

`fields[builds]`

`[string]`

Fields to return for included related types.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`fields[preReleaseVersions]`

`[string]`

Fields to return for included related types.

Possible Values: `version, platform, builds, app`

`filter[app]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[expired]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[id]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[preReleaseVersion]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[processingState]`

`[string]`

Attributes, relationships, and IDs by which to filter.

Possible Values: `PROCESSING, FAILED, INVALID, VALID`

`filter[version]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`include`

`[string]`

Relationship data to include in the response.

Possible Values: `preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`limit[individualTesters]`

`integer`

Number of included related resources to return.

Maximum: `50`

`sort`

`[string]`

Attributes by which to sort.

Possible Values: `version, -version, uploadedDate, -uploadedDate, preReleaseVersion, -preReleaseVersion`

`filter[usesNonExemptEncryption]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[preReleaseVersion.version]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`fields[buildBetaDetails]`

`[string]`

Fields to return for included related types.

Possible Values: `autoNotifyEnabled, internalBuildState, externalBuildState, build`

`filter[betaGroups]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`fields[betaAppReviewSubmissions]`

`[string]`

Fields to return for included related types.

Possible Values: `betaReviewState, submittedDate, build`

`filter[betaAppReviewSubmission.betaReviewState]`

`[string]`

Attributes, relationships, and IDs by which to filter.

Possible Values: `WAITING_FOR_REVIEW, IN_REVIEW, REJECTED, APPROVED`

`fields[betaBuildLocalizations]`

`[string]`

Fields to return for included related types.

Possible Values: `whatsNew, locale, build`

`limit[betaBuildLocalizations]`

`integer`

Number of included related resources to return.

Maximum: `50`

`limit[icons]`

`integer`

Maximum: `50`

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[buildIcons]`

`[string]`

Possible Values: `name, iconAsset, iconType`

`filter[appStoreVersion]`

`[string]`

`filter[preReleaseVersion.platform]`

`[string]`

Possible Values: `IOS, MAC_OS, TV_OS, VISION_OS`

`filter[buildAudienceType]`

`[string]`

Possible Values: `INTERNAL_ONLY, APP_STORE_ELIGIBLE`

`limit[buildBundles]`

`integer`

Maximum: `50`

`limit[betaGroups]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

BuildsResponse

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

Read Build Information

Get information about a specific build.

Read the App Information of a Build

Get the app information for a specific build.

Read the App Store Version Information of a Build

Get the App Store version of a specific build.

Read the Prerelease Version of a Build

Get the prerelease version for a specific build.

Read usage metrics for a beta build

Get usage metrics for a specific build.

