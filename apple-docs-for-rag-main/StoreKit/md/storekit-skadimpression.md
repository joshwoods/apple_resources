

- StoreKit
-  SKAdImpression 

Class

# SKAdImpression

A class that defines an ad impression for a view-through ad.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+

``` source
class SKAdImpression
```

## Mentioned in 

Generating the signature to validate view-through ads

Signing and providing ads

SKAdNetwork 2.2 release notes

## Overview

Create a `SKAdImpression` instance when you’re preparing to present a view-through ad. In the instance, you set:

- Values known to you, including your ad network ID, the App Store IDs of the source app and the advertised app, and the version.

- A value you determine – the campaign ID.

- Values you generate, including the timestamp, a nonce (ad-impression identifier), and the cryptographic signature.

For information about generating the cryptographic signature, see Generating the signature to validate view-through ads.

Use your `SKAdImpression` instance when you call startImpression(_:completionHandler:) to begin presenting your view-through ad. Use the same instance when you call endImpression(_:completionHandler:) to end the ad presentation.

## Topics

### Providing a signature

var signature: String

The advertising network’s cryptographic signature for the ad impression.

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

var timestamp: NSNumber

A number that represents the UNIX time, in milliseconds, of the ad impression.

### Describing ads

var adType: String?

The type of the ad.

var adDescription: String?

A human-readable description of the ad.

var adPurchaserName: String?

The name of the entity that purchased the ad.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Ad impressions and installation validations

Understanding AdAttributionKit and SKAdNetwork interoperability

Learn how attribution APIs interact to deliver ad impressions.

class SKAdNetwork

A class that validates advertisement-driven app installations.

