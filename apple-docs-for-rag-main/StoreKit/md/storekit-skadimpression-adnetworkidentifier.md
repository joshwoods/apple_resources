

- StoreKit
- SKAdImpression
-  adNetworkIdentifier 

Instance Property

# adNetworkIdentifier

A string that represents the advertising network’s unique identifier.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+

``` source
var adNetworkIdentifier: String { get set }
```

## Mentioned in 

Generating the signature to validate view-through ads

Identifying the parameters in install-validation postbacks

## Discussion

Set this property to your ad network ID.

Ad networks obtain an ad network identifier during registration. Ad networks must share their ad network identifiers with participating app developers. Apps that display ads must include the ad network ID in their `Info.plist` to initiate the app install validation process. For more information about acquiring your ad network ID, see Registering an ad network.

## See Also

### Creating a signature

init(sourceAppStoreItemIdentifier: NSNumber, advertisedAppStoreItemIdentifier: NSNumber, adNetworkIdentifier: String, adCampaignIdentifier: NSNumber, adImpressionIdentifier: String, timestamp: NSNumber, signature: String, version: String)

Creates an ad impression object using the supplied values.

var version: String

The version of the SKAdNetwork API.

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

