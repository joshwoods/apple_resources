

- Game Controller
- GCControllerElement
- GCControllerElement.SystemGestureState
-  GCControllerElement.SystemGestureState.alwaysReceive 

Case

# GCControllerElement.SystemGestureState.alwaysReceive

A state that sends input to your app and a gesture recognizer simultaneously.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
case alwaysReceive
```

## Discussion

This state removes any delay in your app receiving the input but may trigger a simultaneous system gesture and in-app action.

## See Also

### States

case enabled

A state that sends input to your app only after a gesture recognizer doesn’t identify a gesture.

case disabled

A state that sends input to your app directly and not to a gesture recognizer.

