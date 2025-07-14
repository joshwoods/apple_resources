

- StoreKit
- SKOverlay
- SKOverlay.AppConfiguration
-  init(appIdentifier:position:) 

Initializer

# init(appIdentifier:position:)

Creates an object that represents the attributes of an overlay you use to recommend another app on the App Store.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
init(
    appIdentifier: String,
    position: SKOverlay.Position
)
```

## Parameters 

`appIdentifier`  

The iTunes identifier of the recommended app.

`position`  

The position of the overlay on the screen.

## See Also

### Creating an App Configuration

var appIdentifier: String

The iTunes identifier of the recommended app.

var position: SKOverlay.Position

The position of the overlay on the screen.

enum Position

Constants that identify the position of an overlay on the screen.

