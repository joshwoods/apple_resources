

- ReplayKit
-  RPBroadcastActivityController 

Class

# RPBroadcastActivityController

A controller object that presents the macOS broadcast picker.

macOS 11.0+

``` source
class RPBroadcastActivityController
```

## Topics

### Showing a Broadcast Picker

class func showBroadcastPicker(at: CGPoint, from: NSWindow?, preferredExtensionIdentifier: String?, completionHandler: (RPBroadcastActivityController?, (any Error)?) -> Void)

Presents a list of available broadcast services for the user to select.

### Accessing the Delegate Object

var delegate: (any RPBroadcastActivityControllerDelegate)?

The broadcast activity controller’s delegate object.

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

### Live Broadcast Implementation

class RPBroadcastActivityViewController

A view controller that displays a user interface where users choose a broadcast service.

class RPSystemBroadcastPickerView

A view displaying a broadcast button that, when tapped, shows a broadcast picker.

protocol RPBroadcastActivityControllerDelegate

A protocol that defines the methods to implement to respond to selection events from a broadcast activity controller.

class RPBroadcastConfiguration

An object used to configure the movie clips produced during a live broadcast.

Deprecated

