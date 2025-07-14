

- AppKit
- NSGestureRecognizerDelegate
-  gestureRecognizerShouldBegin(\_:) 

Instance Method

# gestureRecognizerShouldBegin(\_:)

Asks the delegate if a gesture recognizer should transition out of the Possible (`NSGestureRecognizerStatePossible`) state.

macOS 10.10+

``` source
@MainActor
optional func gestureRecognizerShouldBegin(_ gestureRecognizer: NSGestureRecognizer) -> Bool
```

## Parameters 

`gestureRecognizer`  

The gesture recognizer object that is interpreting events. This is the object with which the delegate is associated.

## Return Value

true to let the gesture recognizer transition out of the Possible (NSGestureRecognizer.State.possible) and continue trying to recognize the gesture or false to prevent it from trying to recognize its gesture. If you do not implement this method, the default return value is true.

## Discussion

When a gesture recognizer attempts to transition from the Possible (NSGestureRecognizer.State.possible) state to a different state, such as NSGestureRecognizer.State.began, the gesture recognizer calls this method to see if the transition should occur. Returning false from this delegate method causes the gesture recognizer to transition to the NSGestureRecognizer.State.failed state.

For information about gesture states and transitions, see State Transitions in NSGestureRecognizer.

## See Also

### Regulating Gesture Recognition

func gestureRecognizer(NSGestureRecognizer, shouldAttemptToRecognizeWith: NSEvent) -> Bool

Asks the delegate if a gesture recognizer should attempt to recognize gestures for a particular event.

