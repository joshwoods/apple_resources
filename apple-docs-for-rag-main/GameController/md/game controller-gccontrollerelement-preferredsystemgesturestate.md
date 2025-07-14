

- Game Controller
- GCControllerElement
-  preferredSystemGestureState 

Instance Property

# preferredSystemGestureState

The preferred state for handling input when the user binds the element to a system gesture.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var preferredSystemGestureState: GCControllerElement.SystemGestureState { get set }
```

## Discussion

In rare situations, you may use this property to disable system gestures. However, the system isn’t guaranteed to respect this property. The default value for this property is GCControllerElement.SystemGestureState.enabled.

## See Also

### Handling system gesture input

var isBoundToSystemGesture: Bool

A Boolean value that indicates whether the user binds the element to a system gesture.

enum SystemGestureState

A state for handling input when an element is part of a system gesture.

