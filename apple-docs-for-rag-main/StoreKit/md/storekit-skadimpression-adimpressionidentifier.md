

- StoreKit
- SKAdImpression
-  adImpressionIdentifier 

Instance Property

# adImpressionIdentifier

A random value to use for added security.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+

``` source
var adImpressionIdentifier: String { get set }
```

## Mentioned in 

Generating the signature to validate view-through ads

## Discussion

Ad networks set the value of this property to a random value (nonce) at the time of the ad impression.

Important

When you generate signature, which is the signature value, you must sign the adImpressionIdentifier as an all-lowercase UUID string representation.

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

var sourceAppStoreItemIdentifier: NSNumber

The App Store ID of the app that displays the ad.

var timestamp: NSNumber

A number that represents the UNIX time, in milliseconds, of the ad impression.

