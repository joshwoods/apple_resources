

- App Store Connect API
-  List Apps 

Web Service Endpoint

# List Apps

Find and list apps in App Store Connect.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps
```

## Query Parameters

`fields[apps]`

`[string]`

Fields to return for included related types.

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[betaLicenseAgreements]`

`[string]`

Fields to return for included related types.

Possible Values: `agreementText, app`

`filter[bundleId]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[id]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[name]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[sku]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`include`

`[string]`

Relationship data to include in the response.

Possible Values: `appEncryptionDeclarations, ciProduct, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, endUserLicenseAgreement, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, gameCenterDetail, appStoreVersionExperimentsV2`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`sort`

`[string]`

Attributes by which to sort.

Possible Values: `name, -name, bundleId, -bundleId, sku, -sku`

`fields[preReleaseVersions]`

`[string]`

Fields to return for included related types.

Possible Values: `version, platform, builds, app`

`limit[preReleaseVersions]`

`integer`

Number of included related resources to return.

Maximum: `50`

`fields[betaAppReviewDetails]`

`[string]`

Fields to return for included related types.

Possible Values: `contactFirstName, contactLastName, contactPhone, contactEmail, demoAccountName, demoAccountPassword, demoAccountRequired, notes, app`

`fields[betaAppLocalizations]`

`[string]`

Fields to return for included related types.

Possible Values: `feedbackEmail, marketingUrl, privacyPolicyUrl, tvOsPrivacyPolicy, description, locale, app`

`fields[builds]`

`[string]`

Fields to return for included related types.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`fields[betaGroups]`

`[string]`

Fields to return for included related types.

Possible Values: `name, createdDate, isInternalGroup, hasAccessToAllBuilds, publicLinkEnabled, publicLinkId, publicLinkLimitEnabled, publicLinkLimit, publicLink, feedbackEnabled, iosBuildsAvailableForAppleSiliconMac, iosBuildsAvailableForAppleVision, app, builds, betaTesters, betaRecruitmentCriteria, betaRecruitmentCriterionCompatibleBuildCheck`

`limit[builds]`

`integer`

Number of included related resources to return.

Maximum: `50`

`limit[betaGroups]`

`integer`

Number of included related resources to return.

Maximum: `50`

`limit[betaAppLocalizations]`

`integer`

Number of included related resources to return.

Maximum: `50`

`limit[appStoreVersions]`

`integer`

Maximum: `50`

`limit[appInfos]`

`integer`

Maximum: `50`

`fields[endUserLicenseAgreements]`

`[string]`

Fields to return for included related types.

Possible Values: `agreementText, app, territories`

`fields[appStoreVersions]`

`[string]`

Fields to return for included related types. Note: `appStoreState` is deprecated, use `appVersionState` instead.

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[appInfos]`

`[string]`

Fields to return for included related types.

Possible Values: `appStoreState, state, appStoreAgeRating, australiaAgeRating, brazilAgeRating, brazilAgeRatingV2, franceAgeRating, koreaAgeRating, kidsAgeBand, app, ageRatingDeclaration, appInfoLocalizations, primaryCategory, primarySubcategoryOne, primarySubcategoryTwo, secondaryCategory, secondarySubcategoryOne, secondarySubcategoryTwo`

`filter[appStoreVersions]`

`[string]`

Fields to return for included related types.

`filter[appStoreVersions.platform]`

`[string]`

Fields to return for included related types.

Possible Values: `IOS, MAC_OS, TV_OS, VISION_OS`

`filter[appStoreVersions.appStoreState]`

`[string]`

Deprecated 

Possible Values: `ACCEPTED, DEVELOPER_REMOVED_FROM_SALE, DEVELOPER_REJECTED, IN_REVIEW, INVALID_BINARY, METADATA_REJECTED, PENDING_APPLE_RELEASE, PENDING_CONTRACT, PENDING_DEVELOPER_RELEASE, PREPARE_FOR_SUBMISSION, PREORDER_READY_FOR_SALE, PROCESSING_FOR_APP_STORE, READY_FOR_REVIEW, READY_FOR_SALE, REJECTED, REMOVED_FROM_SALE, WAITING_FOR_EXPORT_COMPLIANCE, WAITING_FOR_REVIEW, REPLACED_WITH_NEW_VERSION, NOT_APPLICABLE`

`limit[gameCenterEnabledVersions]`

`integer`

Deprecated 

Maximum: `50`

`fields[gameCenterEnabledVersions]`

`[string]`

Deprecated 

Fields to return for included related types.

Possible Values: `platform, versionString, iconAsset, compatibleVersions, app`

`exists[gameCenterEnabledVersions]`

`boolean`

Deprecated 

`limit[inAppPurchases]`

`integer`

Deprecated 

Maximum: `50`

`fields[inAppPurchases]`

`[string]`

Fields to return for included related types.

Possible Values: `referenceName, productId, inAppPurchaseType, state, apps, name, reviewNote, familySharable, contentHosting, inAppPurchaseLocalizations, pricePoints, content, appStoreReviewScreenshot, promotedPurchase, iapPriceSchedule, inAppPurchaseAvailability, images`

`fields[ciProducts]`

`[string]`

Fields to return for included related types.

Possible Values: `name, createdDate, productType, app, bundleId, workflows, primaryRepositories, additionalRepositories, buildRuns`

`limit[appClips]`

`integer`

Maximum: `50`

`fields[appClips]`

`[string]`

Possible Values: `bundleId, app, appClipDefaultExperiences, appClipAdvancedExperiences`

`fields[reviewSubmissions]`

`[string]`

Possible Values: `platform, submittedDate, state, app, items, appStoreVersionForReview, submittedByActor, lastUpdatedByActor`

`fields[appCustomProductPages]`

`[string]`

Possible Values: `name, url, visible, app, appCustomProductPageVersions`

`fields[appEvents]`

`[string]`

Possible Values: `referenceName, badge, eventState, deepLink, purchaseRequirement, primaryLocale, priority, purpose, territorySchedules, archivedTerritorySchedules, localizations`

`limit[appCustomProductPages]`

`integer`

Maximum: `50`

`limit[appEvents]`

`integer`

Maximum: `50`

`limit[reviewSubmissions]`

`integer`

Maximum: `50`

`fields[subscriptionGracePeriods]`

`[string]`

Possible Values: `optIn, sandboxOptIn, duration, renewalType`

`fields[promotedPurchases]`

`[string]`

Possible Values: `visibleForAllUsers, enabled, state, inAppPurchaseV2, subscription`

`fields[subscriptionGroups]`

`[string]`

Possible Values: `referenceName, subscriptions, subscriptionGroupLocalizations`

`limit[inAppPurchasesV2]`

`integer`

Maximum: `50`

`limit[promotedPurchases]`

`integer`

Maximum: `50`

`limit[subscriptionGroups]`

`integer`

Maximum: `50`

`fields[appStoreVersionExperiments]`

`[string]`

Possible Values: `name, platform, trafficProportion, state, reviewRequired, startDate, endDate, app, latestControlVersion, controlVersions, appStoreVersionExperimentTreatments`

`limit[appStoreVersionExperimentsV2]`

`integer`

Maximum: `50`

`fields[appEncryptionDeclarations]`

`[string]`

Possible Values: `appDescription, createdDate, usesEncryption, exempt, containsProprietaryCryptography, containsThirdPartyCryptography, availableOnFrenchStore, platform, uploadedDate, documentUrl, documentName, documentType, appEncryptionDeclarationState, codeValue, app, builds, appEncryptionDeclarationDocument`

`limit[appEncryptionDeclarations]`

`integer`

Maximum: `50`

`fields[gameCenterDetails]`

`[string]`

Possible Values: `arcadeEnabled, challengeEnabled, app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`filter[appStoreVersions.appVersionState]`

`[string]`

This filter is deprecated.

Possible Values: `ACCEPTED, DEVELOPER_REJECTED, IN_REVIEW, INVALID_BINARY, METADATA_REJECTED, PENDING_APPLE_RELEASE, PENDING_DEVELOPER_RELEASE, PREPARE_FOR_SUBMISSION, PROCESSING_FOR_DISTRIBUTION, READY_FOR_DISTRIBUTION, READY_FOR_REVIEW, REJECTED, REPLACED_WITH_NEW_VERSION, WAITING_FOR_EXPORT_COMPLIANCE, WAITING_FOR_REVIEW`

`filter[reviewSubmissions.platform]`

`[string]`

Possible Values: `IOS, MAC_OS, TV_OS, VISION_OS`

`filter[reviewSubmissions.state]`

`[string]`

Possible Values: `READY_FOR_REVIEW, WAITING_FOR_REVIEW, IN_REVIEW, UNRESOLVED_ISSUES, CANCELING, COMPLETING, COMPLETE`

## Response Codes

` 200 ``OK`

AppsResponse

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

## Mentioned in 

Creating alternative distribution packages

Creating keys and establishing alternative marketplace connections

App Store Connect API 3.6 release notes

Creating auto-renewable subscription groups

Creating and configuring keys for web distribution

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps?limit=2
```

```
{
  "data": [
    {
      "type": "apps",
      "id": "10746822401",
      "attributes": {
        "name": "Your Next Cortado",
        "bundleId": "com.bdt.ync",
        "sku": "YNC",
        "primaryLocale": "en-US",
        "isOrEverWasMadeForKids": false,
        "subscriptionStatusUrl": null,
        "subscriptionStatusUrlVersion": null,
        "subscriptionStatusUrlForSandbox": null,
        "subscriptionStatusUrlVersionForSandbox": null,
        "contentRightsDeclaration": "DOES_NOT_USE_THIRD_PARTY_CONTENT",
        "streamlinedBuyEnabled": false
      },
      "relationships": {
        "appEncryptionDeclarations": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/appEncryptionDeclarations",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/appEncryptionDeclarations"
          }
        },
        "ciProduct": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/ciProduct",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/ciProduct"
          }
        },
        "betaTesters": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/betaTesters"
          }
        },
        "betaGroups": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/betaGroups",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/betaGroups"
          }
        },
        "appStoreVersions": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/appStoreVersions",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/appStoreVersions"
          }
        },
        "preReleaseVersions": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/preReleaseVersions",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/preReleaseVersions"
          }
        },
        "betaAppLocalizations": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/betaAppLocalizations",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/betaAppLocalizations"
          }
        },
        "builds": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/builds",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/builds"
          }
        },
        "betaLicenseAgreement": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/betaLicenseAgreement",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/betaLicenseAgreement"
          }
        },
        "betaAppReviewDetail": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/betaAppReviewDetail",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/betaAppReviewDetail"
          }
        },
        "appInfos": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/appInfos",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/appInfos"
          }
        },
        "appClips": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/appClips",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/appClips"
          }
        },
        "appPricePoints": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/appPricePoints",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/appPricePoints"
          }
        },
        "endUserLicenseAgreement": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/endUserLicenseAgreement",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/endUserLicenseAgreement"
          }
        },
        "preOrder": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/preOrder",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/preOrder"
          }
        },
        "appPriceSchedule": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/appPriceSchedule",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/appPriceSchedule"
          }
        },
        "appAvailability": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/appAvailability",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/appAvailability"
          }
        },
        "appAvailabilityV2": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/appAvailabilityV2",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/appAvailabilityV2"
          }
        },
        "inAppPurchases": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/inAppPurchases",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/inAppPurchases"
          }
        },
        "subscriptionGroups": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/subscriptionGroups",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/subscriptionGroups"
          }
        },
        "gameCenterEnabledVersions": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/gameCenterEnabledVersions",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/gameCenterEnabledVersions"
          }
        },
        "perfPowerMetrics": {
          "links": {
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/perfPowerMetrics"
          }
        },
        "appCustomProductPages": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/appCustomProductPages",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/appCustomProductPages"
          }
        },
        "inAppPurchasesV2": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/inAppPurchasesV2",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/inAppPurchasesV2"
          }
        },
        "promotedPurchases": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/promotedPurchases",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/promotedPurchases"
          }
        },
        "appEvents": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/appEvents",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/appEvents"
          }
        },
        "reviewSubmissions": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/reviewSubmissions",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/reviewSubmissions"
          }
        },
        "subscriptionGracePeriod": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/subscriptionGracePeriod",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/subscriptionGracePeriod"
          }
        },
        "customerReviews": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/customerReviews",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/customerReviews"
          }
        },
        "gameCenterDetail": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/gameCenterDetail",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/gameCenterDetail"
          }
        },
        "appStoreVersionExperimentsV2": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/appStoreVersionExperimentsV2",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/appStoreVersionExperimentsV2"
          }
        },
        "alternativeDistributionKey": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/alternativeDistributionKey",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/alternativeDistributionKey"
          }
        },
        "analyticsReportRequests": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/analyticsReportRequests",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/analyticsReportRequests"
          }
        },
        "marketplaceSearchDetail": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/relationships/marketplaceSearchDetail",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746822401/marketplaceSearchDetail"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/apps/10746822401"
      }
    },
    {
      "type": "apps",
      "id": "10746821976",
      "attributes": {
        "name": "A Lot of Latte",
        "bundleId": "com.bdt.latte",
        "sku": "alotoflatte",
        "primaryLocale": "en-US",
        "isOrEverWasMadeForKids": false,
        "subscriptionStatusUrl": null,
        "subscriptionStatusUrlVersion": null,
        "subscriptionStatusUrlForSandbox": null,
        "subscriptionStatusUrlVersionForSandbox": null,
        "contentRightsDeclaration": "DOES_NOT_USE_THIRD_PARTY_CONTENT",
        "streamlinedBuyEnabled": false
      },
      "relationships": {
        "appEncryptionDeclarations": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/appEncryptionDeclarations",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/appEncryptionDeclarations"
          }
        },
        "ciProduct": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/ciProduct",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/ciProduct"
          }
        },
        "betaTesters": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/betaTesters"
          }
        },
        "betaGroups": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/betaGroups",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/betaGroups"
          }
        },
        "appStoreVersions": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/appStoreVersions",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/appStoreVersions"
          }
        },
        "preReleaseVersions": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/preReleaseVersions",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/preReleaseVersions"
          }
        },
        "betaAppLocalizations": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/betaAppLocalizations",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/betaAppLocalizations"
          }
        },
        "builds": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/builds",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/builds"
          }
        },
        "betaLicenseAgreement": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/betaLicenseAgreement",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/betaLicenseAgreement"
          }
        },
        "betaAppReviewDetail": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/betaAppReviewDetail",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/betaAppReviewDetail"
          }
        },
        "appInfos": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/appInfos",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/appInfos"
          }
        },
        "appClips": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/appClips",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/appClips"
          }
        },
        "appPricePoints": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/appPricePoints",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/appPricePoints"
          }
        },
        "endUserLicenseAgreement": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/endUserLicenseAgreement",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/endUserLicenseAgreement"
          }
        },
        "preOrder": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/preOrder",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/preOrder"
          }
        },
        "appPriceSchedule": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/appPriceSchedule",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/appPriceSchedule"
          }
        },
        "appAvailability": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/appAvailability",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/appAvailability"
          }
        },
        "appAvailabilityV2": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/appAvailabilityV2",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/appAvailabilityV2"
          }
        },
        "inAppPurchases": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/inAppPurchases",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/inAppPurchases"
          }
        },
        "subscriptionGroups": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/subscriptionGroups",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/subscriptionGroups"
          }
        },
        "gameCenterEnabledVersions": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/gameCenterEnabledVersions",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/gameCenterEnabledVersions"
          }
        },
        "perfPowerMetrics": {
          "links": {
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/perfPowerMetrics"
          }
        },
        "appCustomProductPages": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/appCustomProductPages",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/appCustomProductPages"
          }
        },
        "inAppPurchasesV2": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/inAppPurchasesV2",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/inAppPurchasesV2"
          }
        },
        "promotedPurchases": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/promotedPurchases",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/promotedPurchases"
          }
        },
        "appEvents": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/appEvents",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/appEvents"
          }
        },
        "reviewSubmissions": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/reviewSubmissions",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/reviewSubmissions"
          }
        },
        "subscriptionGracePeriod": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/subscriptionGracePeriod",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/subscriptionGracePeriod"
          }
        },
        "customerReviews": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/customerReviews",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/customerReviews"
          }
        },
        "gameCenterDetail": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/gameCenterDetail",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/gameCenterDetail"
          }
        },
        "appStoreVersionExperimentsV2": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/appStoreVersionExperimentsV2",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/appStoreVersionExperimentsV2"
          }
        },
        "alternativeDistributionKey": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/alternativeDistributionKey",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/alternativeDistributionKey"
          }
        },
        "analyticsReportRequests": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/analyticsReportRequests",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/analyticsReportRequests"
          }
        },
        "marketplaceSearchDetail": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/relationships/marketplaceSearchDetail",
            "related": "https://api.appstoreconnect.apple.com/v1/apps/10746821976/marketplaceSearchDetail"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/apps/10746821976"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/apps?limit=2",
    "next": "https://api.appstoreconnect.apple.com/v1/apps?cursor=AoJ4g7mg6o4DKzEwNzQ2ODIxOTc2.ANrJC88&limit=2"
  },
  "meta": {
    "paging": {
      "total": 431,
      "limit": 2
    }
  }
}

```

## See Also

### Getting and modifying app information

Read App Information

Get information about a specific app.

Modify an App

Update app information, including bundle ID, primary locale, price schedule, and global availability.

Read an App’s Encryption Declarations

Find and list all available app encryption declarations.

