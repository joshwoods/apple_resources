

- Game Controller
- GCControllerElement
-  GCControllerElement.SystemGestureState 

Enumeration

# GCControllerElement.SystemGestureState

A state for handling input when an element is part of a system gesture.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum SystemGestureState
```

## Topics

### States

case enabled

A state that sends input to your app only after a gesture recognizer doesn’t identify a gesture.

case alwaysReceive

A state that sends input to your app and a gesture recognizer simultaneously.

case disabled

A state that sends input to your app directly and not to a gesture recognizer.

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

### Handling system gesture input

var isBoundToSystemGesture: Bool

A Boolean value that indicates whether the user binds the element to a system gesture.

var preferredSystemGestureState: GCControllerElement.SystemGestureState

The preferred state for handling input when the user binds the element to a system gesture.

