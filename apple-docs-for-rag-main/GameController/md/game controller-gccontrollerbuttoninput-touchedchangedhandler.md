

- Game Controller
- GCControllerButtonInput
-  touchedChangedHandler 

Instance Property

# touchedChangedHandler

The block that the element calls when the user touches the button.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var touchedChangedHandler: GCControllerButtonTouchedChangedHandler? { get set }
```

## Discussion

Set this handler when you want to know when the user touches the button before pressing the button.

## See Also

### Getting change information

typealias GCControllerButtonTouchedChangedHandler

The signature for the block that executes when the user touches the button if the controller supports that feature.

var pressedChangedHandler: GCControllerButtonValueChangedHandler?

The block that the element calls when the user presses or releases the button.

var valueChangedHandler: GCControllerButtonValueChangedHandler?

The block that the element calls when the user changes the level of pressure on the button.

typealias GCControllerButtonValueChangedHandler

The signature for the block that executes when a button’s state changes.

