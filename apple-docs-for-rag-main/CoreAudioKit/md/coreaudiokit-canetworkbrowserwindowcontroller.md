

- CoreAudioKit
-  CANetworkBrowserWindowController 

Class

# CANetworkBrowserWindowController

A window controller that displays available network audio devices.

macOS 10.11+

``` source
@MainActor
class CANetworkBrowserWindowController
```

## Topics

### Creating a Window Controller

init()

Creates a new network browser window controller.

### Determining Audio Video Bridging (AVB) Support

class func isAVBSupported() -> Bool

Returns a Boolean value that indicates whether the current machine hardware supports Audio Video Bridging (AVB).

## Relationships

### Inherits From

- NSWindowController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- Sendable

