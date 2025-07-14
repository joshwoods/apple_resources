

- StoreKit
- SKAdImpression
-  timestamp 

Instance Property

# timestamp

A number that represents the UNIX time, in milliseconds, of the ad impression.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+

``` source
var timestamp: NSNumber { get set }
```

## Mentioned in 

Generating the signature to validate view-through ads

## Discussion

Ad networks generate the timestamp, represented as UNIX time in milliseconds, at the time you begin to serve the ad to users.

## See Also

### Creating a signature

init(sourceAppStoreItemIdentifier: NSNumber, advertisedAppStoreItemIdentifier: NSNumber, adNetworkIdentifier: String, adCampaignIdentifier: NSNumber, adImpressionIdentifier: String, timestamp: NSNumber, signature: String, version: String)

Creates an ad impression object using the supplied values.

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

