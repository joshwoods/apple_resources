

- Game Controller
- GCControllerElement
- GCControllerElement.SystemGestureState
-  GCControllerElement.SystemGestureState.enabled 

Case

# GCControllerElement.SystemGestureState.enabled

A state that sends input to your app only after a gesture recognizer doesn’t identify a gesture.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
case enabled
```

## Discussion

If you enable system gestures, the system sends the input to the gesture recognizer and only sends it to your app if it doesn’t recognize a gesture. If it does recognize a gesture, it doesn’t send any input to your app.

## See Also

### States

case alwaysReceive

A state that sends input to your app and a gesture recognizer simultaneously.

case disabled

A state that sends input to your app directly and not to a gesture recognizer.

