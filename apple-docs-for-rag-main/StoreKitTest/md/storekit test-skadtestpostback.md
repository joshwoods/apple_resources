

- StoreKit Test
-  SKAdTestPostback 

Class

# SKAdTestPostback

A test postback that contains ad conversion information in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
class SKAdTestPostback
```

## Overview

Use this class to create test postbacks to use for unit testing.

In the production environment, the system creates a postback after a user installs an advertised app. The advertised app is responsible for registering the installation and may update the conversion value. The system sends the postback after a timer expires.

In the testing environment, you can mimic a postback by creating it directly. You control the property values within the postback. Use it to test your app’s ability to register the app installation and update conversion values, and to test your server’s ability to receive postbacks.

## Topics

### Creating test postbacks

init?(version: SKAdTestPostbackVersion, adNetworkIdentifier: String, sourceIdentifier: String, appStoreItemIdentifier: Int, sourceAppStoreItemIdentifier: Int, sourceDomain: String?, fidelityType: Int, isRedownload: Bool, didWin: Bool, postbackURL: String)

Creates a test postback for a web ad or an in-app ad.

class func winningPostbacks(withVersion: SKAdTestPostbackVersion, adNetworkIdentifier: String, sourceIdentifier: String, appStoreItemIdentifier: Int, sourceAppStoreItemIdentifier: Int, sourceDomain: String?, fidelityType: Int, isRedownload: Bool, postbackURL: String) -> [SKAdTestPostback]?

Creates a sequence of test postbacks for an in-app or web ad impression.

init?(version: SKAdTestPostbackVersion, adNetworkIdentifier: String, adCampaignIdentifier: Int, appStoreItemIdentifier: Int, sourceAppStoreItemIdentifier: Int, conversionValue: Int, fidelityType: Int, isRedownload: Bool, didWin: Bool, postbackURL: String)

Creates a test postback for an in-app ad.

Deprecated

### Getting the Postback Destination

var postbackURL: String

A URL on your server where the testing environment sends test postbacks.

### Getting general information

var version: SKAdTestPostbackVersion

The SKAdNetwork version that the postback uses.

var transactionIdentifier: String

A unique transaction identifier that the system generates.

var postbackSequenceIndex: Int

The position of this postback among all postbacks for an ad impression.

var isRegistered: Bool

A Boolean value that indicates whether the postback is registered in the testing environment.

var isRedownload: Bool

A Boolean value that indicates whether the user redownloaded and reinstalled the app.

### Getting advertisement information

var adNetworkIdentifier: String

A string that represents the advertising network’s unique identifier.

var appStoreItemIdentifier: Int

The item identifier of the app that this ad impression advertises.

var sourceAppStoreItemIdentifier: Int

The item identifier of the app that displays the ad.

var sourceDomain: String?

The source of a web ad.

var sourceIdentifier: String?

A string that identifies an ad campaign.

### Getting conversion information

var fidelityType: Int

An integer that indicates the type of ad impression, StoreKit-rendered or view-through.

var fineConversionValue: Int

The specific conversion value of an ad postback.

var coarseConversionValue: SKAdNetwork.CoarseConversionValue?

A value that indicates a high, medium, or low conversion value for an ad postback.

var didWin: Bool

A Boolean value that indicates whether the postback won the attribution.

### Getting information in earlier versions

var adCampaignIdentifier: Int

A number that represents the advertising network’s campaign.

var conversionValue: Int

An unsigned 6-bit value that the app or ad network controls.

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

### Ad impression and postback testing

Testing and validating ad impression signatures and postbacks for SKAdNetwork

Validate your ad impressions and test your postbacks by creating unit tests using the StoreKit Test framework.

class SKAdTestSession

The class you use to test ad impressions and postbacks in Xcode.

class SKAdTestPostbackResponse

The status and error information for a postback that the system sends in the testing environment.

struct SKAdTestPostbackVersion

A constant that indicates the postback version.

