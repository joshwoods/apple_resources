

- ReplayKit
-  RPSystemBroadcastPickerView 

Class

# RPSystemBroadcastPickerView

A view displaying a broadcast button that, when tapped, shows a broadcast picker.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class RPSystemBroadcastPickerView
```

## Overview

Add this view to your view hierarchy to let users broadcast directly from your app. When a user taps the broadcast button, it displays a broadcast picker, allowing the user to select a broadcast provider.

Note

Clicking the broadcast button has no effect in Mac apps built with Mac Catalyst.

You can limit the picker to a particular broadcast provider by setting preferredExtension to the bundle identifier of a broadcast extension. You can also show or hide the microphone button displayed in the picker by setting the showsMicrophoneButton property. Set these properties before presenting RPSystemBroadcastPickerView, as shown here:

```
class ViewController: UIViewController {

    @IBOutlet var containerView: UIView!

    override func viewDidLoad() {
        super.viewDidLoad()

        let broadcastPicker = RPSystemBroadcastPickerView(frame: CGRect(x: 0, y: 0, width: 50, height: 50))
        broadcastPicker.preferredExtension = "com.your-app.broadcast.extension"

        containerView.addSubview(broadcastPicker)
    }

}

```

## Topics

### Configuring the Broadcast Picker

var preferredExtension: String?

A bundle identifier of a broadcast extension.

var showsMicrophoneButton: Bool

A Boolean value that indicates whether the microphone button is visible in the broadcast picker.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Live Broadcast Implementation

class RPBroadcastActivityViewController

A view controller that displays a user interface where users choose a broadcast service.

class RPBroadcastActivityController

A controller object that presents the macOS broadcast picker.

protocol RPBroadcastActivityControllerDelegate

A protocol that defines the methods to implement to respond to selection events from a broadcast activity controller.

class RPBroadcastConfiguration

An object used to configure the movie clips produced during a live broadcast.

Deprecated

