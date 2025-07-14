

- Game Controller
- GCControllerElement
- GCControllerElement.SystemGestureState
-  GCControllerElement.SystemGestureState.disabled 

Case

# GCControllerElement.SystemGestureState.disabled

A state that sends input to your app directly and not to a gesture recognizer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
case disabled
```

## Discussion

This state gives your app full control of the input for this element.

## See Also

### States

case enabled

A state that sends input to your app only after a gesture recognizer doesn’t identify a gesture.

case alwaysReceive

A state that sends input to your app and a gesture recognizer simultaneously.

