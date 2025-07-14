

- Game Controller
-  GCControllerButtonValueChangedHandler 

Type Alias

# GCControllerButtonValueChangedHandler

The signature for the block that executes when a button’s state changes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
typealias GCControllerButtonValueChangedHandler = (GCControllerButtonInput, Float, Bool) -> Void
```

## Parameters 

`button`  

The button element whose state changed.

`value`  

A normalized number between `0.0` (minimum) and `1.0` (maximum) that represents the amount of physical or simulated pressure that the user applies to the button.

`pressed`  

A Boolean value that indicates whether the user is pressing the button. If true, the user is pressing the button and the `value` parameter contains the amount of pressure. If false, the user isn’t applying any pressure and the `value` parameter is `0.0`.

## See Also

### Getting change information

var touchedChangedHandler: GCControllerButtonTouchedChangedHandler?

The block that the element calls when the user touches the button.

typealias GCControllerButtonTouchedChangedHandler

The signature for the block that executes when the user touches the button if the controller supports that feature.

var pressedChangedHandler: GCControllerButtonValueChangedHandler?

The block that the element calls when the user presses or releases the button.

var valueChangedHandler: GCControllerButtonValueChangedHandler?

The block that the element calls when the user changes the level of pressure on the button.

