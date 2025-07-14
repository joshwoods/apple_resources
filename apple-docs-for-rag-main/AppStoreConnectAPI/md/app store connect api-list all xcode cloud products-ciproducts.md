

- App Store Connect API
-  List All Xcode Cloud Products 

Web Service Endpoint

# List All Xcode Cloud Products

Get a list of all products you created in Xcode Cloud.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciProducts
```

## Query Parameters

`fields[ciProducts]`

`[string]`

Additional fields to include for each Products resource returned by the response.

Possible Values: `name, createdDate, productType, app, bundleId, workflows, primaryRepositories, additionalRepositories, buildRuns`

`fields[scmRepositories]`

`[string]`

Additional fields to include for each Products resource returned by the response.

Possible Values: `lastAccessedDate, httpCloneUrl, sshCloneUrl, ownerName, repositoryName, scmProvider, defaultBranch, gitReferences, pullRequests`

`filter[app]`

`[string]`

Filter the returned products using the ID of the related Apps resource.

`filter[productType]`

`[string]`

Filter the returned products using the product type attribute.

Possible Values: `APP, FRAMEWORK`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `app, bundleId, primaryRepositories`

`limit`

`integer`

The number of Products resources to return.

Maximum: `200`

`limit[primaryRepositories]`

`integer`

The number of included Products resources to return if the primary repositories relationship is included.

Maximum: `50`

`fields[apps]`

`[string]`

Additional fields to include for each Products resource returned by the response.

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

## Response Codes

` 200 ``OK`

CiProductsResponse

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

## Discussion

The example request below lists ten Xcode Cloud products and sorts the list using the `latestBuildCreatedDate` attribute. Use the information provided in the response to display data about your Xcode Cloud products on a dashboard or to read additional information; for example, workflow information.

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/ciProducts?limit=10&sort=latestBuildCreatedDate
```

```
{
    "data": [
        {
            "type": "ciProducts",
            "id": "cfdc7a3b-0fdf-4463-a0e7-cf9067557beb",
            "attributes": {
                "name": "My Product 5",
                "createdDate": "2021-08-17T18:11:04.616669Z",
                "productType": "APP"
            },
            "relationships": {
                "app": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/cfdc7a3b-0fdf-4463-a0e7-cf9067557beb/relationships/app",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/cfdc7a3b-0fdf-4463-a0e7-cf9067557beb/app"
                    }
                },
                "workflows": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/cfdc7a3b-0fdf-4463-a0e7-cf9067557beb/relationships/workflows",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/cfdc7a3b-0fdf-4463-a0e7-cf9067557beb/workflows"
                    }
                },
                "buildRuns": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/cfdc7a3b-0fdf-4463-a0e7-cf9067557beb/relationships/buildRuns",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/cfdc7a3b-0fdf-4463-a0e7-cf9067557beb/buildRuns"
                    }
                }
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/cfdc7a3b-0fdf-4463-a0e7-cf9067557beb"
            }
        },
        {
            "type": "ciProducts",
            "id": "00c99dd4-fb26-41e7-9aa0-18859cf6d2f7",
            "attributes": {
                "name": "My Product 4",
                "createdDate": "2021-08-17T18:11:04.614927Z",
                "productType": "APP"
            },
            "relationships": {
                "app": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/00c99dd4-fb26-41e7-9aa0-18859cf6d2f7/relationships/app",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/00c99dd4-fb26-41e7-9aa0-18859cf6d2f7/app"
                    }
                },
                "workflows": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/00c99dd4-fb26-41e7-9aa0-18859cf6d2f7/relationships/workflows",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/00c99dd4-fb26-41e7-9aa0-18859cf6d2f7/workflows"
                    }
                },
                "buildRuns": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/00c99dd4-fb26-41e7-9aa0-18859cf6d2f7/relationships/buildRuns",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/00c99dd4-fb26-41e7-9aa0-18859cf6d2f7/buildRuns"
                    }
                }
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/00c99dd4-fb26-41e7-9aa0-18859cf6d2f7"
            }
        },
        {
            "type": "ciProducts",
            "id": "9501b490-307c-46a5-abee-83ae612a7caf",
            "attributes": {
                "name": "My Product 3",
                "createdDate": "2021-08-17T18:11:04.613099Z",
                "productType": "APP"
            },
            "relationships": {
                "app": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/9501b490-307c-46a5-abee-83ae612a7caf/relationships/app",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/9501b490-307c-46a5-abee-83ae612a7caf/app"
                    }
                },
                "workflows": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/9501b490-307c-46a5-abee-83ae612a7caf/relationships/workflows",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/9501b490-307c-46a5-abee-83ae612a7caf/workflows"
                    }
                },
                "buildRuns": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/9501b490-307c-46a5-abee-83ae612a7caf/relationships/buildRuns",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/9501b490-307c-46a5-abee-83ae612a7caf/buildRuns"
                    }
                }
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/9501b490-307c-46a5-abee-83ae612a7caf"
            }
        },
        {
            "type": "ciProducts",
            "id": "d529e42c-f19a-4552-be11-6d74d6211872",
            "attributes": {
                "name": "My Product 2",
                "createdDate": "2021-08-17T18:11:04.611258Z",
                "productType": "APP"
            },
            "relationships": {
                "app": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/d529e42c-f19a-4552-be11-6d74d6211872/relationships/app",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/d529e42c-f19a-4552-be11-6d74d6211872/app"
                    }
                },
                "workflows": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/d529e42c-f19a-4552-be11-6d74d6211872/relationships/workflows",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/d529e42c-f19a-4552-be11-6d74d6211872/workflows"
                    }
                },
                "buildRuns": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/d529e42c-f19a-4552-be11-6d74d6211872/relationships/buildRuns",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/d529e42c-f19a-4552-be11-6d74d6211872/buildRuns"
                    }
                }
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/d529e42c-f19a-4552-be11-6d74d6211872"
            }
        },
        {
            "type": "ciProducts",
            "id": "986a7c7a-a336-4b29-b4ba-de7d3b396be9",
            "attributes": {
                "name": "My Product 1",
                "createdDate": "2021-08-17T18:11:04.609109Z",
                "productType": "APP"
            },
            "relationships": {
                "app": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/986a7c7a-a336-4b29-b4ba-de7d3b396be9/relationships/app",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/986a7c7a-a336-4b29-b4ba-de7d3b396be9/app"
                    }
                },
                "workflows": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/986a7c7a-a336-4b29-b4ba-de7d3b396be9/relationships/workflows",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/986a7c7a-a336-4b29-b4ba-de7d3b396be9/workflows"
                    }
                },
                "buildRuns": {
                    "links": {
                        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/986a7c7a-a336-4b29-b4ba-de7d3b396be9/relationships/buildRuns",
                        "related": "https://api.appstoreconnect.apple.com/v1/ciProducts/986a7c7a-a336-4b29-b4ba-de7d3b396be9/buildRuns"
                    }
                }
            },
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/ciProducts/986a7c7a-a336-4b29-b4ba-de7d3b396be9"
            }
        }
    ],
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/ciProducts?limit=10&sort=latestBuildCreatedDate"
    },
    "meta": {
        "paging": {
            "total": 5,
            "limit": 10
        }
    }
}
```

## See Also

### Getting Xcode Cloud Products

Read Xcode Cloud Product Information

Get information about a specific Xcode Cloud product.

List All Additional Repositories for an Xcode Cloud Product

List all additional Git repositories you associated with an Xcode Cloud product.

Read App Information for an Xcode Cloud Product

Get the app in App Store Connect that’s related to an Xcode Cloud product.

List All Xcode Cloud Builds for an Xcode Cloud Product

List all builds Xcode Cloud performed for a specific product.

List All Primary Git Repositories for an Xcode Cloud Product

List all primary Git repositories for a specific Xcode Cloud product.

List All Workflows for an Xcode Cloud Product

List all workflows for a specific Xcode Cloud product.

Read the Xcode Cloud Product for an App

Get the Xcode Cloud product information for an app you build with Xcode Cloud.

