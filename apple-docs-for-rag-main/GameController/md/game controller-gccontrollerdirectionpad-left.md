

- Game Controller
- GCControllerDirectionPad
-  left 

Instance Property

# left

The button element that changes the negative x-axis.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var left: GCControllerButtonInput { get }
```

## Discussion

The value of the `right` and `left` buttons are mutually exclusive because the user can only press one of these buttons at a time. Therefore, when the `left` button is nonzero, the `right` button is `0`.

## See Also

### Accessing values using directional buttons

var right: GCControllerButtonInput

The button element that changes the positive x-axis.

var up: GCControllerButtonInput

The button element that changes the positive y-axis.

var down: GCControllerButtonInput

The button element used for the negative y-axis direction.

