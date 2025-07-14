

- Game Controller
- GCControllerTouchpad
-  touchSurface 

Instance Property

# touchSurface

The element that represents the state of the user’s touch on the surface of the touchpad.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var touchSurface: GCControllerDirectionPad { get }
```

## Discussion

This element provides the recent or last touch positions on the two axes. Use the touchState property to determine whether the user is currently touching the surface.

## See Also

### Getting the subelements

var button: GCControllerButtonInput

The element that represents the button component on the touchpad.

