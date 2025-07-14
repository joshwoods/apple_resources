

- WatchKit
- WKGestureRecognizer
-  isEnabled 

Instance Property

# isEnabled

A Boolean value indicating whether the gesture recognizer is enabled.

watchOS 3.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

When the value of this property is true, the gesture recognizer actively tracks touches and reports state changes to its action method. When the value of this property is false, the gesture recognizer does not track events or call its action method. The default value of this property is true.

If you change the value of this property to false while the gesture recognizer is in the middle of tracking touch events, the gesture recognizer transitions to the WKGestureRecognizerState.cancelled state.

## See Also

### Getting the Gesture Recognizer’s State

var state: WKGestureRecognizerState

The current state of the gesture recognizer.

