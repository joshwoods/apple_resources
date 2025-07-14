

- StoreKit
-  SKCloudServiceCapability Deprecated

Structure

# SKCloudServiceCapability

Constants that specify the current capabilities of the customer’s Music library on the device.

iOS 9.3–18.0DeprecatediPadOS 9.3–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 9.3–18.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct SKCloudServiceCapability
```

Deprecated

Use MusicSubscription from MusicKit

## Topics

### Initializing

init(rawValue: UInt)

Initializes a cloud service capability with the provided raw value.

### Identifying Cloud Service Capabilities

static var musicCatalogPlayback: SKCloudServiceCapability

The device allows playback of Apple Music catalog tracks.

static var musicCatalogSubscriptionEligible: SKCloudServiceCapability

The device allows subscription to the Apple Music catalog.

static var addToCloudMusicLibrary: SKCloudServiceCapability

The device allows tracks to be added to the user’s music library.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Determining capabilities

Determining a person’s Apple Music capabilities

Determine which Apple Music capabilities are available on a customer’s device.

func requestUserToken(forDeveloperToken: String, completionHandler: (String?, (any Error)?) -> Void)

Returns a user token that you use to access personalized Apple Music content.

Deprecated

func requestStorefrontCountryCode(completionHandler: (String?, (any Error)?) -> Void)

Gets the country code for the storefront associated with a customer’s iTunes account.

Deprecated

func requestCapabilities(completionHandler: (SKCloudServiceCapability, (any Error)?) -> Void)

Gets the current capabilities associated with the Music library on the device.

Deprecated

func requestStorefrontIdentifier(completionHandler: (String?, (any Error)?) -> Void)

Gets the device’s storefront identifier.

Deprecated

func requestPersonalizationToken(forClientToken: String, withCompletionHandler: (String?, (any Error)?) -> Void)Deprecated

