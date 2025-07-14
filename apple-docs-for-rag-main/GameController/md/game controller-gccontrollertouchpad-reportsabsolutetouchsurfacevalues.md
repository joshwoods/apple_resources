

- Game Controller
- GCControllerTouchpad
-  reportsAbsoluteTouchSurfaceValues 

Instance Property

# reportsAbsoluteTouchSurfaceValues

A Boolean value that determines whether the touch values are absolute or relative.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var reportsAbsoluteTouchSurfaceValues: Bool { get set }
```

## Discussion

If this property is true, the touch values are absolute on the surface of the touchpad. If this property is false, the touch values are relative to the first touch on a virtual directional pad. The default value for this property is true.

## See Also

### Accessing the input values

var touchState: GCControllerTouchpad.TouchState

The state of the user’s touch on the surface of the touchpad.

enum TouchState

The possible states of the user’s touch.

