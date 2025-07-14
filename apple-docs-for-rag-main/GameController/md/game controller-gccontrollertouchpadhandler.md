

- Game Controller
-  GCControllerTouchpadHandler 

Type Alias

# GCControllerTouchpadHandler

The signature for the block that executes when the user interacts with the touchpad.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
typealias GCControllerTouchpadHandler = (GCControllerTouchpad, Float, Float, Float, Bool) -> Void
```

## Parameters 

`touchpad`  

The touchpad that the user interacts with.

`xValue`  

A normalized value of the x-axis touch location ranging from `-1` to `1`.

`yValue`  

A normalized value of the y-axis touch location ranging from `-1` to `1`.

`buttonValue`  

A normalized number between `0.0` (minimum) and `1.0` (maximum) that represents the level of pressure the user applies to the touchpad button.

`buttonPressed`  

A Boolean value that indicates whether the user is pressing the touchpad button. If true, the user is pressing the button; otherwise, the user isn’t.

## See Also

### Getting change information

var touchDown: GCControllerTouchpadHandler?

The block that the element calls when the user begins touching the touchpad.

var touchMoved: GCControllerTouchpadHandler?

The block that the element calls when the user continues touching the touchpad, not when the user begins or ends touching the touchpad.

var touchUp: GCControllerTouchpadHandler?

The block that the element calls when the user finishes touching the touchpad.

