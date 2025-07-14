

- Game Controller
- GCControllerTouchpad
-  touchUp 

Instance Property

# touchUp

The block that the element calls when the user finishes touching the touchpad.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var touchUp: GCControllerTouchpadHandler? { get set }
```

## Discussion

The element invokes this handler when the user removes their fingers from the touchpad.

## See Also

### Getting change information

var touchDown: GCControllerTouchpadHandler?

The block that the element calls when the user begins touching the touchpad.

var touchMoved: GCControllerTouchpadHandler?

The block that the element calls when the user continues touching the touchpad, not when the user begins or ends touching the touchpad.

typealias GCControllerTouchpadHandler

The signature for the block that executes when the user interacts with the touchpad.

