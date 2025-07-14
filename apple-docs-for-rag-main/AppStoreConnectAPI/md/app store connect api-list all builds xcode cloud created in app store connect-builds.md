

- App Store Connect API
-  List All Builds Xcode Cloud Created in App Store Connect 

Web Service Endpoint

# List All Builds Xcode Cloud Created in App Store Connect

List All App Store Connect and TestFlight Builds when it performed a build.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciBuildRuns/{id}/builds
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Build Runs resource.

## Query Parameters

`fields[betaBuildLocalizations]`

`[string]`

Additional fields to include for each Builds resource returned by the response.

Possible Values: `whatsNew, locale, build`

`fields[betaTesters]`

`[string]`

Additional fields to include for each Builds resource returned by the response.

Possible Values: `firstName, lastName, email, inviteType, state, apps, betaGroups, builds`

`fields[buildIcons]`

`[string]`

Additional fields to include for each Builds resource returned by the response.

Possible Values: `name, iconAsset, iconType`

`fields[builds]`

`[string]`

Additional fields to include for each Builds resource returned by the response.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`filter[appStoreVersion]`

`[string]`

Filter the returned builds using the ID of the related App Store Versions resource.

`filter[app]`

`[string]`

Filter the returned builds using the ID of the related Apps resource.

`filter[betaAppReviewSubmission.betaReviewState]`

`[string]`

Filter the returned builds using the beta review state attribute.

Possible Values: `WAITING_FOR_REVIEW, IN_REVIEW, REJECTED, APPROVED`

`filter[betaGroups]`

`[string]`

Filter the returned builds using the ID of the related Beta Groups resource.

`filter[expired]`

`[string]`

Filter the returned builds using the expired attribute.

`filter[id]`

`[string]`

Filter the returned builds using the ID of the Builds resource.

`filter[preReleaseVersion.platform]`

`[string]`

Filter the returned builds using the platform attribute of the Pre-Release Versions resource.

Possible Values: `IOS, MAC_OS, TV_OS, VISION_OS`

`filter[preReleaseVersion.version]`

`[string]`

Filter the returned builds using the version attribute of the Pre-Release Versions resource.

`filter[preReleaseVersion]`

`[string]`

Filter the returned builds using the ID of the related Pre-Release Versions resource.

`filter[processingState]`

`[string]`

Filter the returned builds using the processing state attribute.

Possible Values: `PROCESSING, FAILED, INVALID, VALID`

`filter[usesNonExemptEncryption]`

`[string]`

Filter the returned builds using the uses nonexempt encryption attribute.

`filter[version]`

`[string]`

Filter the returned builds using the version attribute.

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles`

`limit`

`integer`

The number of Builds resources to return.

Maximum: `200`

`limit[betaBuildLocalizations]`

`integer`

The number of included Builds resources to return if the beta build localization relationship is included.

Maximum: `50`

`limit[icons]`

`integer`

The number of included Builds resources to return if the icons relationship is included.

Maximum: `50`

`limit[individualTesters]`

`integer`

The number of included Builds resources to return if the individual testers relationship is included.

Maximum: `50`

`sort`

`[string]`

Attributes by which to sort the returned Builds resources.

Possible Values: `version, -version, uploadedDate, -uploadedDate, preReleaseVersion, -preReleaseVersion`

`filter[buildAudienceType]`

`[string]`

Possible Values: `INTERNAL_ONLY, APP_STORE_ELIGIBLE`

`limit[buildBundles]`

`integer`

Maximum: `50`

`fields[buildBundles]`

`[string]`

Possible Values: `bundleId, bundleType, sdkBuild, platformBuild, fileName, hasSirikit, hasOnDemandResources, hasPrerenderedIcon, usesLocationServices, isIosBuildMacAppStoreCompatible, includesSymbols, dSYMUrl, supportedArchitectures, requiredCapabilities, deviceProtocols, locales, entitlements, appClipDomainCacheStatus, appClipDomainDebugStatus, betaAppClipInvocations, buildBundleFileSizes`

`fields[betaGroups]`

`[string]`

Possible Values: `name, createdDate, isInternalGroup, hasAccessToAllBuilds, publicLinkEnabled, publicLinkId, publicLinkLimitEnabled, publicLinkLimit, publicLink, feedbackEnabled, iosBuildsAvailableForAppleSiliconMac, iosBuildsAvailableForAppleVision, app, builds, betaTesters, betaRecruitmentCriteria, betaRecruitmentCriterionCompatibleBuildCheck`

`limit[betaGroups]`

`integer`

Maximum: `50`

`fields[betaAppReviewSubmissions]`

`[string]`

Possible Values: `betaReviewState, submittedDate, build`

`fields[buildBetaDetails]`

`[string]`

Possible Values: `autoNotifyEnabled, internalBuildState, externalBuildState, build`

`fields[preReleaseVersions]`

`[string]`

Possible Values: `version, platform, builds, app`

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[appEncryptionDeclarations]`

`[string]`

Possible Values: `appDescription, createdDate, usesEncryption, exempt, containsProprietaryCryptography, containsThirdPartyCryptography, availableOnFrenchStore, platform, uploadedDate, documentUrl, documentName, documentType, appEncryptionDeclarationState, codeValue, app, builds, appEncryptionDeclarationDocument`

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

## Response Codes

` 200 ``OK`

BuildsResponse

`OK`

The request completed successfully.

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

### Getting Build Information

Read Xcode Cloud Build Information

Get information about a specific Xcode Cloud build.

List All Actions for an Xcode Cloud Build

List all actions Xcode Cloud performed during a specific build.

