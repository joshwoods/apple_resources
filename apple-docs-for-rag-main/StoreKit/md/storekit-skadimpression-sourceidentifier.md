

- StoreKit
- SKAdImpression
-  sourceIdentifier 

Instance Property

# sourceIdentifier

A four-digit integer that ad networks define to represent the ad campaign.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
var sourceIdentifier: NSNumber { get set }
```

## Mentioned in 

Generating the signature to validate view-through ads

SKAdNetwork 4 release notes

Identifying the parameters in install-validation postbacks

## Discussion

The sourceIdentifier key is available for ad impressions that use SKAdNetwork 4 and later. The sourceIdentifier, also known as the *hierarchical source identifier*, replaces and extends the campaign identifier value, adCampaignIdentifier.

Ad networks and developers define the meaning of the hierarchical source identifier. This integer can have up to four digits. You can encode information about your advertisement in each set of digits; you may receive two, three, or all four digits of the sourceIdentifier in the first winning postback, depending on the ad impression’s postback data tier. For more information about the value you may get in the postback, see Receiving postbacks in multiple conversion windows.

Note

An install-validation postback represents this integer as a string in its `source-identifier` parameter. For more details about the parameters of an install-validation postback, see Identifying the parameters in install-validation postbacks.

## See Also

### Creating a signature

init(sourceAppStoreItemIdentifier: NSNumber, advertisedAppStoreItemIdentifier: NSNumber, adNetworkIdentifier: String, adCampaignIdentifier: NSNumber, adImpressionIdentifier: String, timestamp: NSNumber, signature: String, version: String)

Creates an ad impression object using the supplied values.

var version: String

The version of the SKAdNetwork API.

var adNetworkIdentifier: String

A string that represents the advertising network’s unique identifier.

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

