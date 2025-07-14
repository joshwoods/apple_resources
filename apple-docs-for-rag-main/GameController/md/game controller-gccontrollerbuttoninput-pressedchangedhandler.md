

- Game Controller
- GCControllerButtonInput
-  pressedChangedHandler 

Instance Property

# pressedChangedHandler

The block that the element calls when the user presses or releases the button.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var pressedChangedHandler: GCControllerButtonValueChangedHandler? { get set }
```

## Discussion

Set this handler when you only want to know when the user presses or releases the button — that is, when the isPressed property changes.

## See Also

### Getting change information

var touchedChangedHandler: GCControllerButtonTouchedChangedHandler?

The block that the element calls when the user touches the button.

typealias GCControllerButtonTouchedChangedHandler

The signature for the block that executes when the user touches the button if the controller supports that feature.

var valueChangedHandler: GCControllerButtonValueChangedHandler?

The block that the element calls when the user changes the level of pressure on the button.

typealias GCControllerButtonValueChangedHandler

The signature for the block that executes when a button’s state changes.

