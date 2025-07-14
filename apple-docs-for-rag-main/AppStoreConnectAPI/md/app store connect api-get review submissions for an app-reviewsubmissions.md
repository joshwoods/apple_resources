

- App Store Connect API
-  Get review submissions for an app 

Web Service Endpoint

# Get review submissions for an app

Get a list of review submissions associated with a specific app.

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/reviewSubmissions
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[reviewSubmissionItems]`

`[string]`

Possible Values: `state, appStoreVersion, appCustomProductPageVersion, appStoreVersionExperiment, appStoreVersionExperimentV2, appEvent`

`fields[reviewSubmissions]`

`[string]`

Possible Values: `platform, submittedDate, state, app, items, appStoreVersionForReview, submittedByActor, lastUpdatedByActor`

`filter[platform]`

`[string]`

Possible Values: `IOS, MAC_OS, TV_OS, VISION_OS`

`filter[state]`

`[string]`

Possible Values: `READY_FOR_REVIEW, WAITING_FOR_REVIEW, IN_REVIEW, UNRESOLVED_ISSUES, CANCELING, COMPLETING, COMPLETE`

`include`

`[string]`

Possible Values: `app, items, appStoreVersionForReview, submittedByActor, lastUpdatedByActor`

`limit`

`integer`

Maximum: `200`

`limit[items]`

`integer`

Maximum: `50`

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[actors]`

`[string]`

Possible Values: `actorType, userFirstName, userLastName, userEmail, apiKeyId`

## Response Codes

` 200 ``OK`

ReviewSubmissionsResponse

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/6446998023/reviewSubmissions
```

```
{
    "data": [
        {
            "type": "reviewSubmissions",
            "id": "fda9bd85-170b-4a1c-8d78-c2b445527542",
            "attributes": {
                "platform": "IOS",
                "submittedDate": null,
                "state": "READY_FOR_REVIEW"
            },
            "relationships": {
                "items": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/reviewSubmissions/fda9bd85-170b-4a1c-8d78-c2b445527542/relationships/items",
                        "related": "https://api.appstoreconnect.apple.com/v1/reviewSubmissions/fda9bd85-170b-4a1c-8d78-c2b445527542/items"
                    }
                }
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/reviewSubmissions/fda9bd85-170b-4a1c-8d78-c2b445527542"
            }
        }
    ],
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/reviewSubmissions"
    },
    "meta": {
        "paging": {
            "total": 1,
            "limit": 50
        }
    }
}

```

