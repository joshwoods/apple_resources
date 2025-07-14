

- StoreKit
- SKOverlay
-  SKOverlay.AppConfiguration 

Class

# SKOverlay.AppConfiguration

An object that represents the attributes of an overlay you use to recommend another app on the App Store.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class AppConfiguration
```

## Topics

### Creating an App Configuration

init(appIdentifier: String, position: SKOverlay.Position)

Creates an object that represents the attributes of an overlay you use to recommend another app on the App Store.

var appIdentifier: String

The iTunes identifier of the recommended app.

var position: SKOverlay.Position

The position of the overlay on the screen.

enum Position

Constants that identify the position of an overlay on the screen.

### Dismissing the Overlay

var userDismissible: Bool

A Boolean value that indicates whether the user can dismiss the overlay.

### Verifying Advertising Campaigns

var campaignToken: String?

A token you use to represent an ad campaign and measure its effectiveness.

var providerToken: String?

A token that represents the provider of an app promotion campaign, and that you use to measure the campaign’s effectiveness.

func setAdditionalValue(Any?, forKey: String)

Sets an additional value for a key; for example, a value for measuring the effectiveness of an ad campaign.

func additionalValue(forKey: String) -> Any?

Returns the object associated with the key.

### Promoting the Latest App Version

var latestReleaseID: String?

The release ID of the latest version of your app as displayed in App Store Connect.

### Advertising Another App

var customProductPageIdentifier: String?

An optional identifier for an app’s custom product page.

### Setting an Ad Impression

func setAdImpression(SKAdImpression)

### Instance Properties

var adAttributionReengagementURL: URL?

var appImpression: AppImpression?

## Relationships

### Inherits From

- SKOverlay.Configuration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Creating an overlay

init(configuration: SKOverlay.Configuration)

Creates an overlay you use to recommend another app on the App Store.

var configuration: SKOverlay.Configuration

An overlay’s attributes; for example, its position on the screen.

class AppClipConfiguration

An object that represents the attributes of an overlay you use to recommend an App Clip’s corresponding full app.

class Configuration

The abstract superclass for all classes that represent an overlay’s attributes.

