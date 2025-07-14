

- StoreKit
- SKAdImpression
-  sourceAppStoreItemIdentifier 

Instance Property

# sourceAppStoreItemIdentifier

The App Store ID of the app that displays the ad.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+

``` source
var sourceAppStoreItemIdentifier: NSNumber { get set }
```

## Mentioned in 

Generating the signature to validate view-through ads

Identifying the parameters in install-validation postbacks

## Discussion

Set this property to the App Store item identifier of the app that’s displaying the ad.

If you’re using a development-signed build to display the ads and not an app from App Store during testing, use `0` as the item identifier.

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

var timestamp: NSNumber

A number that represents the UNIX time, in milliseconds, of the ad impression.

