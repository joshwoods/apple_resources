

- UIKit
- UIScreen
-  mirrored 

Instance Property

# mirrored

The screen an external display mirrors from.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+tvOS

``` source
@MainActor
var mirrored: UIScreen? { get }
```

## Discussion

When a screen supports mirroring and mirroring is active, this property contains the screen object associated with the device’s main screen. This represents the screen the attached display mirrors from. The value of this property is `nil` when mirroring is disabled, not supported, or no screen is connected to the device.

To disable mirroring and use the external display for presenting unique content, create a window and associate it with a windowExternalDisplayNonInteractive scene.

## See Also

### Related Documentation

class var main: UIScreen

Returns the screen object representing the device’s screen.

Deprecated

### Detecting screen capture

var isCaptured: Bool

A Boolean value that indicates whether the system is actively cloning the screen to another destination.

Deprecated

