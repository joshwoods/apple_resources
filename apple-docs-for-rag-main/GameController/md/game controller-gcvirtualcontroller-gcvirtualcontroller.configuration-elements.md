

- Game Controller
- GCVirtualController
- GCVirtualController.Configuration
-  elements 

Instance Property

# elements

The input elements of a virtual controller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var elements: Set { get set }
```

## Mentioned in 

Adding touch controls to games that support game controllers in iOS

## Discussion

The possible values you can include in this array are the names of the following constants: GCInputButtonA, GCInputButtonB, GCInputButtonX, GCInputButtonY, GCInputDirectionPad, GCInputLeftThumbstick, GCInputRightThumbstick, GCInputLeftShoulder, GCInputRightShoulder, GCInputLeftTrigger, and GCInputRightTrigger.

Note

If you include both `GCInputDirectionPad` and `GCInputLeftThumbstick` in the array, the virtual controller contains only the left thumb stick, not the input direction pad.

For example, configure a virtual controller with a left thumb stick, right thumb stick, A button, and B button.

```
virtualConfiguration.elements = [GCInputLeftThumbstick,GCInputRightThumbstick,GCInputButtonA,GCInputButtonB]
```

