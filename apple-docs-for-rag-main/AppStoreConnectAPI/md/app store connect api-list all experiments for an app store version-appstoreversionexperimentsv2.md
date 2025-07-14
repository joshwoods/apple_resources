

- App Store Connect API
-  List All Experiments for an App Store Version 

Web Service Endpoint

# List All Experiments for an App Store Version

Get a list of all experiments for an App Store version of an app across all platforms.

App Store Connect API 2.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/appStoreVersionExperimentsV2
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List All App Store Versions for an App response.

## Query Parameters

`fields[appStoreVersionExperimentTreatments]`

`[string]`

Possible Values: `name, appIcon, appIconName, promotedDate, appStoreVersionExperiment, appStoreVersionExperimentV2, appStoreVersionExperimentTreatmentLocalizations`

`fields[appStoreVersionExperiments]`

`[string]`

Possible Values: `name, platform, trafficProportion, state, reviewRequired, startDate, endDate, app, latestControlVersion, controlVersions, appStoreVersionExperimentTreatments`

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`filter[state]`

`[string]`

Possible Values: `PREPARE_FOR_SUBMISSION, READY_FOR_REVIEW, WAITING_FOR_REVIEW, IN_REVIEW, ACCEPTED, APPROVED, REJECTED, COMPLETED, STOPPED`

`include`

`[string]`

Possible Values: `app, latestControlVersion, controlVersions, appStoreVersionExperimentTreatments`

`limit`

`integer`

Maximum: `200`

`limit[appStoreVersionExperimentTreatments]`

`integer`

Maximum: `50`

`limit[controlVersions]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppStoreVersionExperimentsV2Response

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

App Store Connect API 2.4 release notes

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/appStoreVersions/fb3bb89c-47c3-4cbf-8af7-677fb801c09f/appStoreVersionExperimentsV2
```

```
{
  "data" : [ {
    "type" : "appStoreVersionExperiments",
    "id" : "1a22d9a7-f574-4669-b1ca-1ba88f786c19",
    "attributes" : {
      "name" : "PPO Test 1",
      "platform" : "IOS",
      "trafficProportion" : 50,
      "state" : "READY_FOR_REVIEW",
      "reviewRequired" : true,
      "startDate" : null,
      "endDate" : null
    },
    "relationships" : {
      "appStoreVersionExperimentTreatments" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19/relationships/appStoreVersionExperimentTreatments",
          "related" : "https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19/appStoreVersionExperimentTreatments"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/appStoreVersionExperiments/1a22d9a7-f574-4669-b1ca-1ba88f786c19"
    }
  } ],
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/appStoreVersions/fb3bb89c-47c3-4cbf-8af7-677fb801c09f/appStoreVersionExperimentsV2"
  },
  "meta" : {
    "paging" : {
      "total" : 1,
      "limit" : 50
    }
  }
}
```

## See Also

### Getting App Store Version Experiments

List All Experiments for an App Store Version v1

Get a list of all experiments for an App Store version of an app across all platforms.

Deprecated

