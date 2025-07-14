

- StoreKit
- SKOverlay
-  init(configuration:) 

Initializer

# init(configuration:)

Creates an overlay you use to recommend another app on the App Store.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
init(configuration: SKOverlay.Configuration)
```

## Parameters 

`configuration`  

The object that represents the overlay’s attributes; for example, its position on the screen.

## Discussion

Pass an SKOverlay.AppConfiguration as the `configuration` parameter if you want to display the overlay in an app. To recommend an App Clip’s corresponding app, pass an SKOverlay.AppClipConfiguration object to the initializer. For more information, see Recommending your app to App Clip users.

## See Also

### Creating an overlay

var configuration: SKOverlay.Configuration

An overlay’s attributes; for example, its position on the screen.

class AppConfiguration

An object that represents the attributes of an overlay you use to recommend another app on the App Store.

class AppClipConfiguration

An object that represents the attributes of an overlay you use to recommend an App Clip’s corresponding full app.

class Configuration

The abstract superclass for all classes that represent an overlay’s attributes.

