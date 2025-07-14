

- Game Controller
- GCControllerButtonInput
-  valueChangedHandler 

Instance Property

# valueChangedHandler

The block that the element calls when the user changes the level of pressure on the button.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var valueChangedHandler: GCControllerButtonValueChangedHandler? { get set }
```

## Discussion

Set this handler when you want to know when the pressure level changes.

## See Also

### Getting change information

var touchedChangedHandler: GCControllerButtonTouchedChangedHandler?

The block that the element calls when the user touches the button.

typealias GCControllerButtonTouchedChangedHandler

The signature for the block that executes when the user touches the button if the controller supports that feature.

var pressedChangedHandler: GCControllerButtonValueChangedHandler?

The block that the element calls when the user presses or releases the button.

typealias GCControllerButtonValueChangedHandler

The signature for the block that executes when a button’s state changes.

