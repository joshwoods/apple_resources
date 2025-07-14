

- App Store Connect API
-  Read the Build Information of a Build Beta Detail 

Web Service Endpoint

# Read the Build Information of a Build Beta Detail

Get the build information for a specific build beta details resource.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/buildBetaDetails/{id}/build
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`fields[builds]`

`[string]`

Fields to return for included related types.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`fields[appEncryptionDeclarations]`

`[string]`

Possible Values: `appDescription, createdDate, usesEncryption, exempt, containsProprietaryCryptography, containsThirdPartyCryptography, availableOnFrenchStore, platform, uploadedDate, documentUrl, documentName, documentType, appEncryptionDeclarationState, codeValue, app, builds, appEncryptionDeclarationDocument`

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[betaAppReviewSubmissions]`

`[string]`

Possible Values: `betaReviewState, submittedDate, build`

`fields[betaBuildLocalizations]`

`[string]`

Possible Values: `whatsNew, locale, build`

`fields[betaGroups]`

`[string]`

Possible Values: `name, createdDate, isInternalGroup, hasAccessToAllBuilds, publicLinkEnabled, publicLinkId, publicLinkLimitEnabled, publicLinkLimit, publicLink, feedbackEnabled, iosBuildsAvailableForAppleSiliconMac, iosBuildsAvailableForAppleVision, app, builds, betaTesters, betaRecruitmentCriteria, betaRecruitmentCriterionCompatibleBuildCheck`

`fields[betaTesters]`

`[string]`

Possible Values: `firstName, lastName, email, inviteType, state, apps, betaGroups, builds`

`fields[buildBetaDetails]`

`[string]`

Possible Values: `autoNotifyEnabled, internalBuildState, externalBuildState, build`

`fields[buildBundles]`

`[string]`

Possible Values: `bundleId, bundleType, sdkBuild, platformBuild, fileName, hasSirikit, hasOnDemandResources, hasPrerenderedIcon, usesLocationServices, isIosBuildMacAppStoreCompatible, includesSymbols, dSYMUrl, supportedArchitectures, requiredCapabilities, deviceProtocols, locales, entitlements, appClipDomainCacheStatus, appClipDomainDebugStatus, betaAppClipInvocations, buildBundleFileSizes`

`fields[buildIcons]`

`[string]`

Possible Values: `name, iconAsset, iconType`

`fields[preReleaseVersions]`

`[string]`

Possible Values: `version, platform, builds, app`

`include`

`[string]`

Possible Values: `preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles`

`limit[betaBuildLocalizations]`

`integer`

Maximum: `50`

`limit[betaGroups]`

`integer`

Maximum: `50`

`limit[buildBundles]`

`integer`

Maximum: `50`

`limit[icons]`

`integer`

Maximum: `50`

`limit[individualTesters]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

BuildResponse

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

Read Build Beta Detail Information

Get a specific build beta details resource.

