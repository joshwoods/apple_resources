

- StoreKit
- SKAdImpression
-  adCampaignIdentifier 

Instance Property

# adCampaignIdentifier

A number that represents the advertising network’s campaign.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+

``` source
var adCampaignIdentifier: NSNumber { get set }
```

## Mentioned in 

Generating the signature to validate view-through ads

Identifying the parameters in install-validation postbacks

## Discussion

Ad networks set their own campaign identifiers, which must be an integer `>=1` and `

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

var advertisedAppStoreItemIdentifier: NSNumber

The App Store ID of the app that the ad impression advertises.

var adImpressionIdentifier: String

A random value to use for added security.

var sourceAppStoreItemIdentifier: NSNumber

The App Store ID of the app that displays the ad.

var timestamp: NSNumber

A number that represents the UNIX time, in milliseconds, of the ad impression.

