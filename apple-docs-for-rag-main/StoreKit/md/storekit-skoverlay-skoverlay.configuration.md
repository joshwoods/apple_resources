

- StoreKit
- SKOverlay
-  SKOverlay.Configuration 

Class

# SKOverlay.Configuration

The abstract superclass for all classes that represent an overlay’s attributes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class Configuration
```

## Relationships

### Inherits From

- NSObject

### Inherited By

- SKOverlay.AppClipConfiguration
- SKOverlay.AppConfiguration

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

class AppClipConfiguration

An object that represents the attributes of an overlay you use to recommend an App Clip’s corresponding full app.

