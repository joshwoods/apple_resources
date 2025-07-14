

- ReplayKit
-  RPBroadcastActivityControllerDelegate 

Protocol

# RPBroadcastActivityControllerDelegate

A protocol that defines the methods to implement to respond to selection events from a broadcast activity controller.

macOS 11.0+

``` source
protocol RPBroadcastActivityControllerDelegate : NSObjectProtocol
```

## Topics

### Responding to User Selection

func broadcastActivityController(RPBroadcastActivityController, didFinishWith: RPBroadcastController?, error: (any Error)?)

Tells the delegate that a user selected a broadcast.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Live Broadcast Implementation

class RPBroadcastActivityViewController

A view controller that displays a user interface where users choose a broadcast service.

class RPSystemBroadcastPickerView

A view displaying a broadcast button that, when tapped, shows a broadcast picker.

class RPBroadcastActivityController

A controller object that presents the macOS broadcast picker.

class RPBroadcastConfiguration

An object used to configure the movie clips produced during a live broadcast.

Deprecated

