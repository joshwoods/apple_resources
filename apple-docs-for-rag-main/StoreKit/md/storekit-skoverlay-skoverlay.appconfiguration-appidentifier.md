

- StoreKit
- SKOverlay
- SKOverlay.AppConfiguration
-  appIdentifier 

Instance Property

# appIdentifier

The iTunes identifier of the recommended app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var appIdentifier: String { get set }
```

## See Also

### Creating an App Configuration

init(appIdentifier: String, position: SKOverlay.Position)

Creates an object that represents the attributes of an overlay you use to recommend another app on the App Store.

var position: SKOverlay.Position

The position of the overlay on the screen.

enum Position

Constants that identify the position of an overlay on the screen.

