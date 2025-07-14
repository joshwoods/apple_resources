

- Game Controller
- GCControllerButtonInput
-  value 

Instance Property

# value

The level of pressure the user is applying to the button.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var value: Float { get }
```

## Discussion

If the user applies pressure to the button, the isPressed property is true and this property indicates the amount of pressure. The framework normalizes the value to a number between `0.0` (minimum) and `1.0` (maximum). If the user isn’t pressing the button, the isPressed property is false and this property is `0.0`.

For axis buttons, such as thumbsticks and touchpads, the location on the positive or negative axis of the element simulates the pressure.

## See Also

### Accessing input values

var isTouched: Bool

A Boolean value that indicates whether the user is touching the button.

var isPressed: Bool

A Boolean value that indicates whether the user is pressing the button.

