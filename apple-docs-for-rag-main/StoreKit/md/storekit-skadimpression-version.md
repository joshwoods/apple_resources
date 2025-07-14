

- StoreKit
- SKAdImpression
-  version 

Instance Property

# version

The version of the SKAdNetwork API.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+

``` source
var version: String { get set }
```

## Mentioned in 

Generating the signature to validate view-through ads

Identifying the parameters in install-validation postbacks

## Discussion

Set this instance property to the SKAdNetwork version you’re using to sign the view-through ad impression. View-through ads are available starting in version 2.2. For more information about versions and availability, see SKAdNetwork release notes.

## See Also

### Creating a signature

init(sourceAppStoreItemIdentifier: NSNumber, advertisedAppStoreItemIdentifier: NSNumber, adNetworkIdentifier: String, adCampaignIdentifier: NSNumber, adImpressionIdentifier: String, timestamp: NSNumber, signature: String, version: String)

Creates an ad impression object using the supplied values.

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

