

- Game Controller
-  GCControllerButtonTouchedChangedHandler 

Type Alias

# GCControllerButtonTouchedChangedHandler

The signature for the block that executes when the user touches the button if the controller supports that feature.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
typealias GCControllerButtonTouchedChangedHandler = (GCControllerButtonInput, Float, Bool, Bool) -> Void
```

## Parameters 

`button`  

The button element whose value changed.

`value`  

A normalized number between `0.0` (minimum) and `1.0` (maximum) that represents the amount of physical or simulated pressure that the user applies to the button.

`pressed`  

A Boolean value that indicates whether the user is pressing the button. If true, the user is pressing the button and the `value` parameter contains the amount of pressure. If false, the user isn’t applying any pressure and the `value` parameter is `0.0`.

`touched`  

A Boolean value that indicates whether the user is touching the button. If true, the user is touching the button; otherwise, the user isn’t.

## See Also

### Getting change information

var touchedChangedHandler: GCControllerButtonTouchedChangedHandler?

The block that the element calls when the user touches the button.

var pressedChangedHandler: GCControllerButtonValueChangedHandler?

The block that the element calls when the user presses or releases the button.

var valueChangedHandler: GCControllerButtonValueChangedHandler?

The block that the element calls when the user changes the level of pressure on the button.

typealias GCControllerButtonValueChangedHandler

The signature for the block that executes when a button’s state changes.

