

- Game Controller
- GCMouseInput
-  auxiliaryButtons 

Instance Property

# auxiliaryButtons

The optional additional buttons on the mouse.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var auxiliaryButtons: [GCControllerButtonInput]? { get }
```

## Discussion

If the mouse doesn’t have additional buttons, this property is `nil`.

## See Also

### Accessing Buttons

var leftButton: GCControllerButtonInput

The left button on the mouse.

var rightButton: GCControllerButtonInput?

The optional right button on the mouse.

var middleButton: GCControllerButtonInput?

The optional middle button on the mouse.

