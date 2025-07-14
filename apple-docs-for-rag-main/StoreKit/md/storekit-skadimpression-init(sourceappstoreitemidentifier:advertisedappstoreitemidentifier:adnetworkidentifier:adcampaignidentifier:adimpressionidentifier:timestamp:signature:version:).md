

- StoreKit
- SKAdImpression
-  init(sourceAppStoreItemIdentifier:advertisedAppStoreItemIdentifier:adNetworkIdentifier:adCampaignIdentifier:adImpressionIdentifier:timestamp:signature:version:) 

Initializer

# init(sourceAppStoreItemIdentifier:advertisedAppStoreItemIdentifier:adNetworkIdentifier:adCampaignIdentifier:adImpressionIdentifier:timestamp:signature:version:)

Creates an ad impression object using the supplied values.

iOS 16.0+iPadOS 16.0+

``` source
init(
    sourceAppStoreItemIdentifier: NSNumber,
    advertisedAppStoreItemIdentifier: NSNumber,
    adNetworkIdentifier: String,
    adCampaignIdentifier: NSNumber,
    adImpressionIdentifier: String,
    timestamp: NSNumber,
    signature: String,
    version: String
)
```

## See Also

### Creating a signature

var version: String

The version of the SKAdNetwork API.

var adNetworkIdentifier: String

A string that represents the advertising network’s unique identifier.

var sourceIdentifier: NSNumber

A four-digit integer that ad networks define to represent the ad campaign.

var adCampaignIdentifier: NSNumber

A number that represents the advertising network’s campaign.

var advertisedAppStoreItemIdentifier: NSNumber

The App Store ID of the app that the ad impression advertises.

var adImpressionIdentifier: String

A random value to use for added security.

var sourceAppStoreItemIdentifier: NSNumber

The App Store ID of the app that displays the ad.

var timestamp: NSNumber

A number that represents the UNIX time, in milliseconds, of the ad impression.

