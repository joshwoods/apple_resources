

- WatchKit
- WKGestureRecognizer
-  state 

Instance Property

# state

The current state of the gesture recognizer.

watchOS 3.0+

``` source
var state: WKGestureRecognizerState { get }
```

## Discussion

As the gesture recognizer processes touch events, it updates the value of this property. Some states apply only to gestures that comprise a continuous sequences of touch events that must be tracked over time, such as pan gestures.

## See Also

### Getting the Gesture Recognizer’s State

var isEnabled: Bool

A Boolean value indicating whether the gesture recognizer is enabled.

