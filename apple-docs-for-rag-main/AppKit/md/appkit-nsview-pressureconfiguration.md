

- AppKit
- NSView
-  pressureConfiguration 

Instance Property

# pressureConfiguration

Configures the behavior and progression of the Force Touch trackpad when responding to touch input produced by the user when the cursor is over the view.

macOS 10.11+

``` source
@MainActor
var pressureConfiguration: NSPressureConfiguration? { get set }
```

## Discussion

This property configures the behavior and progression of the Force Touch trackpad when responding to touch input produced by the user when the cursor is over the view.

Changing the value of this property does not affect a pressure event that’s already active. This property must be set prior to a mouse-down event, for use with future pressure gestures.

## See Also

### Related Documentation

class NSPressureConfiguration

An encapsulation of the behavior and progression of a Force Touch trackpad as it responds to specific events.

enum PressureBehavior

These constants describe the behavior and progression of a pressure gesture.

init(pressureBehavior: NSEvent.PressureBehavior)

Initializes a pressure configuration object with a specified pressure behavior.

