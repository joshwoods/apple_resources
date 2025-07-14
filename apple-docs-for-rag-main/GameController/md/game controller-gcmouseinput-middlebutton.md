

- Game Controller
- GCMouseInput
-  middleButton 

Instance Property

# middleButton

The optional middle button on the mouse.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var middleButton: GCControllerButtonInput? { get }
```

## Discussion

If the mouse doesn’t have a middle button, this property is `nil`.

## See Also

### Accessing Buttons

var leftButton: GCControllerButtonInput

The left button on the mouse.

var rightButton: GCControllerButtonInput?

The optional right button on the mouse.

var auxiliaryButtons: [GCControllerButtonInput]?

The optional additional buttons on the mouse.

