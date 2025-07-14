

- App Store Connect API
-  List All App Store Versions for an App 

Web Service Endpoint

# List All App Store Versions for an App

Get a list of all App Store versions of an app across all platforms.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/appStoreVersions
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the apps resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`include`

`[string]`

Relationship data to include in the response. Note: `ageRatingDeclaration` is deprecated.

Possible Values: `app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, alternativeDistributionPackage`

`fields[apps]`

`[string]`

Fields to return for included related types.

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[appStoreVersionSubmissions]`

`[string]`

Fields to return for included related types.

Value: `appStoreVersion`

`fields[builds]`

`[string]`

Fields to return for included related types.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`fields[appStoreVersions]`

`[string]`

Fields to return for included related types. Note: `ageRatingDeclaration` is deprecated.

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[appStoreReviewDetails]`

`[string]`

Fields to return for included related types.

Possible Values: `contactFirstName, contactLastName, contactPhone, contactEmail, demoAccountName, demoAccountPassword, demoAccountRequired, notes, appStoreVersion, appStoreReviewAttachments`

`fields[ageRatingDeclarations]`

`[string]`

Deprecated. To get age rating declarations, use Read age rating declaration instead.

Possible Values: `alcoholTobaccoOrDrugUseOrReferences, contests, gamblingAndContests, gambling, gamblingSimulated, kidsAgeBand, lootBox, medicalOrTreatmentInformation, profanityOrCrudeHumor, sexualContentGraphicAndNudity, sexualContentOrNudity, horrorOrFearThemes, matureOrSuggestiveThemes, unrestrictedWebAccess, violenceCartoonOrFantasy, violenceRealisticProlongedGraphicOrSadistic, violenceRealistic, ageRatingOverride, koreaAgeRatingOverride, seventeenPlus`

`fields[appStoreVersionPhasedReleases]`

`[string]`

Fields to return for included related types.

Possible Values: `phasedReleaseState, startDate, totalPauseDuration, currentDayNumber`

`fields[routingAppCoverages]`

`[string]`

Fields to return for included related types.

Possible Values: `fileSize, fileName, sourceFileChecksum, uploadOperations, assetDeliveryState, appStoreVersion`

`fields[appStoreVersionLocalizations]`

`[string]`

Fields to return for included related types.

Possible Values: `description, locale, keywords, marketingUrl, promotionalText, supportUrl, whatsNew, appStoreVersion, appScreenshotSets, appPreviewSets`

`filter[id]`

`[string]`

Fields to return for included related types.

`filter[versionString]`

`[string]`

Fields to return for included related types.

`filter[platform]`

`[string]`

Fields to return for included related types.

Possible Values: `IOS, MAC_OS, TV_OS, VISION_OS`

`filter[appStoreState]`

`[string]`

Deprecated 

Fields to return for included related types.

Possible Values: `ACCEPTED, DEVELOPER_REMOVED_FROM_SALE, DEVELOPER_REJECTED, IN_REVIEW, INVALID_BINARY, METADATA_REJECTED, PENDING_APPLE_RELEASE, PENDING_CONTRACT, PENDING_DEVELOPER_RELEASE, PREPARE_FOR_SUBMISSION, PREORDER_READY_FOR_SALE, PROCESSING_FOR_APP_STORE, READY_FOR_REVIEW, READY_FOR_SALE, REJECTED, REMOVED_FROM_SALE, WAITING_FOR_EXPORT_COMPLIANCE, WAITING_FOR_REVIEW, REPLACED_WITH_NEW_VERSION, NOT_APPLICABLE`

`limit[appStoreVersionLocalizations]`

`integer`

Maximum: `50`

`fields[appStoreVersionExperiments]`

`[string]`

Possible Values: `name, trafficProportion, state, reviewRequired, startDate, endDate, appStoreVersion, appStoreVersionExperimentTreatments, platform, app, latestControlVersion, controlVersions`

`limit[appStoreVersionExperiments]`

`integer`

Deprecated 

Maximum: `50`

`fields[appClipDefaultExperiences]`

`[string]`

Possible Values: `action, appClip, releaseWithAppStoreVersion, appClipDefaultExperienceLocalizations, appClipAppStoreReviewDetail`

`limit[appStoreVersionExperimentsV2]`

`integer`

Maximum: `50`

`filter[appVersionState]`

`[string]`

Possible Values: `ACCEPTED, DEVELOPER_REJECTED, IN_REVIEW, INVALID_BINARY, METADATA_REJECTED, PENDING_APPLE_RELEASE, PENDING_DEVELOPER_RELEASE, PREPARE_FOR_SUBMISSION, PROCESSING_FOR_DISTRIBUTION, READY_FOR_DISTRIBUTION, READY_FOR_REVIEW, REJECTED, REPLACED_WITH_NEW_VERSION, WAITING_FOR_EXPORT_COMPLIANCE, WAITING_FOR_REVIEW`

`fields[alternativeDistributionPackages]`

`[string]`

Value: `versions`

`fields[gameCenterAppVersions]`

`[string]`

Possible Values: `enabled, compatibilityVersions, appStoreVersion`

## Response Codes

` 200 ``OK`

AppStoreVersionsResponse

`OK`

Request succeeded.

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

## Mentioned in 

Creating alternative distribution packages

App Store Connect API 1.3 release notes

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/6446998023/appStoreVersions
```

```
{
  "data": [
    {
      "type": "appStoreVersions",
      "id": "2395b439-fccd-4645-95bc-97afbe9e379e",
      "attributes": {
        "platform": "IOS",
        "versionString": "1.0",
        "appStoreState": "PREPARE_FOR_SUBMISSION",
        "copyright": "2022 YNC",
        "releaseType": "MANUAL",
        "earliestReleaseDate": null,
        "usesIdfa": null,
        "downloadable": true,
        "createdDate": "2022-08-31T09:28:28-07:00"
      },
      "relationships": {
        "ageRatingDeclaration": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/relationships/ageRatingDeclaration",
            "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/ageRatingDeclaration"
          }
        },
        "appStoreVersionLocalizations": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/relationships/appStoreVersionLocalizations",
            "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/appStoreVersionLocalizations"
          }
        },
        "build": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/relationships/build",
            "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/build"
          }
        },
        "appStoreVersionPhasedRelease": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/relationships/appStoreVersionPhasedRelease",
            "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/appStoreVersionPhasedRelease"
          }
        },
        "routingAppCoverage": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/relationships/routingAppCoverage",
            "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/routingAppCoverage"
          }
        },
        "appStoreReviewDetail": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/relationships/appStoreReviewDetail",
            "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/appStoreReviewDetail"
          }
        },
        "appStoreVersionSubmission": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/relationships/appStoreVersionSubmission",
            "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/appStoreVersionSubmission"
          }
        },
        "idfaDeclaration": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/relationships/idfaDeclaration",
            "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/idfaDeclaration"
          }
        },
        "appClipDefaultExperience": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/relationships/appClipDefaultExperience",
            "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/appClipDefaultExperience"
          }
        },
        "appStoreVersionExperiments": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/relationships/appStoreVersionExperiments",
            "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/appStoreVersionExperiments"
          }
        },
        "customerReviews": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/relationships/customerReviews",
            "related": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e/customerReviews"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/appStoreVersions/2395b439-fccd-4645-95bc-97afbe9e379e"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/appStoreVersions"
  },
  "meta": {
    "paging": {
      "total": 1,
      "limit": 50
    }
  }
}
```

## See Also

### Getting App Store details for your app

List All App Infos for an App

Get information about an app that is currently live on App Store, or that goes live with the next version.

Read the End User License Agreement Information of an App

Get the custom end user license agreement (EULA) for a specific app and the territories where the agreement applies.

List all custom product pages for an app

Get a list of all custom product pages for a specific app.

GET /v1/apps/{id}/appStoreVersionExperimentsV2

