

- Game Controller
- GCControllerTouchpad
-  touchDown 

Instance Property

# touchDown

The block that the element calls when the user begins touching the touchpad.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var touchDown: GCControllerTouchpadHandler? { get set }
```

## See Also

### Getting change information

var touchMoved: GCControllerTouchpadHandler?

The block that the element calls when the user continues touching the touchpad, not when the user begins or ends touching the touchpad.

var touchUp: GCControllerTouchpadHandler?

The block that the element calls when the user finishes touching the touchpad.

typealias GCControllerTouchpadHandler

The signature for the block that executes when the user interacts with the touchpad.

