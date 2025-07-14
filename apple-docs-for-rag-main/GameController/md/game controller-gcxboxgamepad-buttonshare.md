

- Game Controller
- GCXboxGamepad
-  buttonShare 

Instance Property

# buttonShare

The share button on an Xbox Series X\|S controller or later.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var buttonShare: GCControllerButtonInput? { get }
```

## Discussion

The system reserves the Share button for screenshot and video recording gestures. If you want to disable these gestures in your app, set the button’s preferredSystemGestureState to GCControllerElement.SystemGestureState.disabled.

## See Also

### Getting button inputs

var paddleButton1: GCControllerButtonInput?

The controller’s paddle 1 button element, which has a P1 label on the back of the controller.

var paddleButton2: GCControllerButtonInput?

The paddle 2 button element, which has a P2 label on the back of the controller.

var paddleButton3: GCControllerButtonInput?

The paddle 3 button element, which has a P3 label on the back of the controller.

var paddleButton4: GCControllerButtonInput?

The paddle 4 button element, which has a P4 label on the back of the controller.

