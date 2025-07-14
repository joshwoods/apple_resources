

- ReplayKit
-  RPBroadcastConfiguration Deprecated

Class

# RPBroadcastConfiguration

An object used to configure the movie clips produced during a live broadcast.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 10.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class RPBroadcastConfiguration
```

Deprecated

No longer supported

## Topics

### Configuring Movie Clips

var clipDuration: TimeInterval

The duration of movie clips sent the to the movie clip handler extension.

var videoCompressionProperties: [String : any NSSecureCoding &amp; NSObjectProtocol]?

The compression properties for encoding movie clips that are to be overwritten.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Live Broadcast Implementation

class RPBroadcastActivityViewController

A view controller that displays a user interface where users choose a broadcast service.

class RPSystemBroadcastPickerView

A view displaying a broadcast button that, when tapped, shows a broadcast picker.

class RPBroadcastActivityController

A controller object that presents the macOS broadcast picker.

protocol RPBroadcastActivityControllerDelegate

A protocol that defines the methods to implement to respond to selection events from a broadcast activity controller.

