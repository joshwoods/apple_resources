

- Game Controller
- GCControllerTouchpad
-  GCControllerTouchpad.TouchState 

Enumeration

# GCControllerTouchpad.TouchState

The possible states of the user’s touch.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum TouchState
```

## Topics

### States

case up

The user stops or isn’t touching the surface.

case down

The user starts touching the surface.

case moving

The user continues touching the surface.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing the input values

var touchState: GCControllerTouchpad.TouchState

The state of the user’s touch on the surface of the touchpad.

var reportsAbsoluteTouchSurfaceValues: Bool

A Boolean value that determines whether the touch values are absolute or relative.

