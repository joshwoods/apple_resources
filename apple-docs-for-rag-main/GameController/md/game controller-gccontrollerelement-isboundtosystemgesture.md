

- Game Controller
- GCControllerElement
-  isBoundToSystemGesture 

Instance Property

# isBoundToSystemGesture

A Boolean value that indicates whether the user binds the element to a system gesture.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var isBoundToSystemGesture: Bool { get }
```

## Discussion

This property is true if the user binds this element to a gesture; otherwise, it’s false.

## See Also

### Handling system gesture input

var preferredSystemGestureState: GCControllerElement.SystemGestureState

The preferred state for handling input when the user binds the element to a system gesture.

enum SystemGestureState

A state for handling input when an element is part of a system gesture.

