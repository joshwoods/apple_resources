

- StoreKit
- SKOverlay
- SKOverlay.AppConfiguration
-  position 

Instance Property

# position

The position of the overlay on the screen.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var position: SKOverlay.Position { get set }
```

## See Also

### Creating an App Configuration

init(appIdentifier: String, position: SKOverlay.Position)

Creates an object that represents the attributes of an overlay you use to recommend another app on the App Store.

var appIdentifier: String

The iTunes identifier of the recommended app.

enum Position

Constants that identify the position of an overlay on the screen.

