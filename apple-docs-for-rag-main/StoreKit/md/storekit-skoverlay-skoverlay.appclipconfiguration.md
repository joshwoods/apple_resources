

- StoreKit
- SKOverlay
-  SKOverlay.AppClipConfiguration 

Class

# SKOverlay.AppClipConfiguration

An object that represents the attributes of an overlay you use to recommend an App Clip’s corresponding full app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class AppClipConfiguration
```

## Topics

### Creating an App Clip Configuration

init(position: SKOverlay.Position)

Creates an object that represents the attributes of an overlay you use to recommend an App Clip’s corresponding app.

var position: SKOverlay.Position

The position of the overlay on the screen.

enum Position

Constants that identify the position of an overlay on the screen.

### Verifying Advertising Campaigns

var campaignToken: String?

A token you use to represent an ad campaign and measure its effectiveness.

var providerToken: String?

A token that represents the provider of an app promotion campaign, and that you use to measure the campaign’s effectiveness.

func setAdditionalValue(Any?, forKey: String)

Sets an additional value for a key, such as a value for measuring the effectiveness of an ad campaign.

func additionalValue(forKey: String) -> Any?

Returns the object associated with the key.

### Promoting the Latest App Version

var latestReleaseID: String?

The release ID of the latest version of your parent app as displayed in App Store Connect.

### Advertising Another App

var customProductPageIdentifier: String?

An identifier for a parent app’s custom product page.

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

class AppConfiguration

An object that represents the attributes of an overlay you use to recommend another app on the App Store.

class Configuration

The abstract superclass for all classes that represent an overlay’s attributes.

