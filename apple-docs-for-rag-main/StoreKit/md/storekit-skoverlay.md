

- StoreKit
-  SKOverlay 

Class

# SKOverlay

A class that displays an overlay you can use to recommend another app or an App Clip’s corresponding full app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class SKOverlay
```

## Mentioned in 

Signing and providing ads

Receiving ad attributions and postbacks

## Overview

By displaying an overlay, you can recommend another app to users and enable them to download it immediately. To recommend media that’s not an app, or to display a product page within your app, use SKStoreProductViewController.

Important

If you display an overlay in your App Clip, you may only recommend the App Clip’s corresponding full app and need to initialize the overlay with an SKOverlay.AppClipConfiguration object. For more information, see Recommending your app to App Clip users.

If you’re using SwiftUI, make use of the `appStoreOverlay(isPresented:configuration:)` modifier. For example usage, see Fruta: Building a Feature-Rich App with SwiftUI.

To display an App Store overlay in an app that uses UIKit:

1.  Create an SKOverlay.AppConfiguration with the iTunes identifier of the app you want to recommend.

2.  Initialize `SKOverlay` with the configuration object.

3.  Present the overlay.

The following code displays an overlay at the bottom of the visible scene:

```
func displayOverlay() {
    guard let scene = view.window?.windowScene else { return }

    let config = SKOverlay.AppConfiguration(appIdentifier: "The iTunes identifier of another app.", position: .bottom)
    let overlay = SKOverlay(configuration: config)
    overlay.present(in: scene)
}
```

To respond to the overlay’s appearance, dismissal, or failure to load, set the delegate and implement the methods defined in SKOverlayDelegate.

Note

App extensions can’t display an overlay.

## Topics

### Creating an overlay

init(configuration: SKOverlay.Configuration)

Creates an overlay you use to recommend another app on the App Store.

var configuration: SKOverlay.Configuration

An overlay’s attributes; for example, its position on the screen.

class AppConfiguration

An object that represents the attributes of an overlay you use to recommend another app on the App Store.

class AppClipConfiguration

An object that represents the attributes of an overlay you use to recommend an App Clip’s corresponding full app.

class Configuration

The abstract superclass for all classes that represent an overlay’s attributes.

### Presenting an overlay

func present(in: UIWindowScene)

Presents an overlay in a window scene.

### Dismissing an overlay

class func dismiss(in: UIWindowScene)

Dismisses an App Store overlay.

### Setting a delegate

var delegate: (any SKOverlayDelegate)?

The overlay’s delegate.

protocol SKOverlayDelegate

Methods for responding to the overlay’s appearance, dismissal, or failure to load.

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

### Recommendations

Offering media for sale in your app

Allow users to purchase media in the App Store from within your app.

class SKStoreProductViewController

A view controller that provides a page where customers can purchase media from the App Store.

