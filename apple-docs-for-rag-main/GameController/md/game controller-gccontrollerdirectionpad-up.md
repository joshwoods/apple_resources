

- Game Controller
- GCControllerDirectionPad
-  up 

Instance Property

# up

The button element that changes the positive y-axis.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var up: GCControllerButtonInput { get }
```

## Discussion

The value of the `up` and `down` buttons are mutually exclusive because the user can only press one of these buttons at a time. Therefore, when the `up` button is nonzero, the `down` button is `0`.

## See Also

### Accessing values using directional buttons

var right: GCControllerButtonInput

The button element that changes the positive x-axis.

var left: GCControllerButtonInput

The button element that changes the negative x-axis.

var down: GCControllerButtonInput

The button element used for the negative y-axis direction.

