

- Game Controller
- GCControllerButtonInput
-  isTouched 

Instance Property

# isTouched

A Boolean value that indicates whether the user is touching the button.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var isTouched: Bool { get }
```

## Discussion

If this property is true, the user is touching the button; otherwise, the user isn’t. For controllers that support capacitive touch, the user can start touching the button without pressure when the value property is `0`. For controllers that don’t support capacitive touch, the user starts touching the button when the value property is greater than `0`.

## See Also

### Accessing input values

var isPressed: Bool

A Boolean value that indicates whether the user is pressing the button.

var value: Float

The level of pressure the user is applying to the button.

