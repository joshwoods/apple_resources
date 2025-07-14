

- Technotes
-  TN3180: Reverting to App Store Server Notifications V1 

Article

# TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

## Overview

When you enable your server to receive App Store Server Notifications, you configure your settings in App Store Connect. You select the version of App Store Server Notifications you want to receive, and provide your server URL, as described in Enter server URLs for App Store Server Notifications.

Note

The App Store Server Notifications V1 endpoint and version 1 notifications are deprecated. Implement the App Store Server Notifications V2 endpoint on your server to receive version 2 notifications instead.

In the unusual case that you need to revert from version 2 to version 1 of App Store Server Notifications, use the Modify an App endpoint.

## Create the app modification request

The Modify an App endpoint updates app information including the URL and version you use for App Store Notifications. To use this endpoint, create a object that includes the `id`, `type`, and `attributes` properties detailed in AppUpdateRequest.Data.

To revert to version 1 of App Store Server Notifications, add the following attributes to the request body of the endpoint:

| Attribute | Value |
|----|----|
| `subscriptionStatusUrl` | Your server’s App Store Server Notifications V1 endpoint URL. |
| `subscriptionStatusUrlVersion` | `V1` to indicate you’re using version 1 of App Store Server Notifications. |

The following code shows an example of a modification request that changes only the app’s App Store Server Notifications URL and version:

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/6446998023 -d
"{
    "data": {
        "type": "apps",
        "id": "6446998023",
        "attributes": {
            "subscriptionStatusUrl": "https://myserver.example.com",
            "subscriptionStatusUrlVersion": "V1"
        }
    }
}"

```

```
{
    "data": {
        "type": "apps",
        "id": "6446998023",
        "attributes": {
            "name": "Your Next Cortado",
            "bundleId": "com.bdt.ync",
            "sku": "YNC",
            "primaryLocale": "en-US",
            "isOrEverWasMadeForKids": false,
            "subscriptionStatusUrl": "https://myserver.example.com",
            "subscriptionStatusUrlVersion": "V1",
            "subscriptionStatusUrlForSandbox": null,
            "subscriptionStatusUrlVersionForSandbox": null,
            "availableInNewTerritories": true,
            "contentRightsDeclaration": "DOES_NOT_USE_THIRD_PARTY_CONTENT"
        },
        "relationships": {
            "ciProduct": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/ciProduct",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/ciProduct"
                }
            },
            "betaTesters": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/betaTesters"
                }
            },
            "betaGroups": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/betaGroups",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/betaGroups"
                }
            },
            "appStoreVersions": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/appStoreVersions",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/appStoreVersions"
                }
            },
            "preReleaseVersions": {
                "links": {
                     "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/preReleaseVersions",
                     "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/preReleaseVersions"
                }
            },
            "betaAppLocalizations": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/betaAppLocalizations",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/betaAppLocalizations"
                }
            },
            "builds": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/builds",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/builds"
                }
            },
            "betaLicenseAgreement": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/betaLicenseAgreement",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/betaLicenseAgreement"
                }
            },
            "betaAppReviewDetail": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/betaAppReviewDetail",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/betaAppReviewDetail"
                }
            },
            "appInfos": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/appInfos",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/appInfos"
                }
            },
            "appClips": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/appClips",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/appClips"
                }
            },
            "appPricePoints": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/appPricePoints",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/appPricePoints"
                }
            },
            "pricePoints": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/pricePoints",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/pricePoints"
                }
            },
            "endUserLicenseAgreement": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/endUserLicenseAgreement",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/endUserLicenseAgreement"
                }
            },
            "preOrder": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/preOrder",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/preOrder"
                }
            },
            "prices": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/prices",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/prices"
                }
            },
            "appPriceSchedule": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/appPriceSchedule",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/appPriceSchedule"
                }
            },
            "availableTerritories": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/availableTerritories",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/availableTerritories"
                }
            },
            "appAvailability": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/appAvailability",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/appAvailability"
                }
            },
            "inAppPurchases": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/inAppPurchases",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/inAppPurchases"
                }
            },
            "subscriptionGroups": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/subscriptionGroups",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/subscriptionGroups"
                }
            },
            "gameCenterEnabledVersions": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/gameCenterEnabledVersions",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/gameCenterEnabledVersions"
                }
            },
            "perfPowerMetrics": {
                "links": {
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/perfPowerMetrics"
                }
            },
            "appCustomProductPages": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/appCustomProductPages",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/appCustomProductPages"
                }
            },
            "inAppPurchasesV2": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/inAppPurchasesV2",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/inAppPurchasesV2"
                }
            },
            "promotedPurchases": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/promotedPurchases",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/promotedPurchases"
                }
            },
            "appEvents": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/appEvents",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/appEvents"
                }
            },
            "reviewSubmissions": {
                "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/reviewSubmissions",
                "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/reviewSubmissions"
                }
            },
            "subscriptionGracePeriod": {
            "links": {
                "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/subscriptionGracePeriod",
                "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/subscriptionGracePeriod"
                }
            },
            "customerReviews": {
                "links": {
                    "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/relationships/customerReviews",
                    "related": "https://api.appstoreconnect.apple.com/v1/apps/6446998023/customerReviews"
                }
            }
        },
        "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023"
        }
    },
    "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/apps/6446998023"
    }
}
```

To change your server’s URL for receiving App Store Server Notifications in the sandbox environment, add the following attributes to the request body of the endpoint:

| Attribute | Value |
|----|----|
| `subscriptionStatusUrlForSandbox` | Your server’s App Store Server Notifications V1 endpoint URL for the sandbox environment. |
| `subscriptionStatusUrlVersionForSandbox` | `V1` to indicate you’re using version 1 of App Store Server Notifications in the sandbox environment. |

## Revision History

- **2024-11-12** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

TN3158: Resolving Xcode 15 device connection issues

Identify software preventing Xcode 15 from connecting to Apple devices, and modify your configuration to allow these connections.

