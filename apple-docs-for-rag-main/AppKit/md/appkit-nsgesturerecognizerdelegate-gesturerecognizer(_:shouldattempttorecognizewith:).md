

- AppKit
- NSGestureRecognizerDelegate
-  gestureRecognizer(\_:shouldAttemptToRecognizeWith:) 

Instance Method

# gestureRecognizer(\_:shouldAttemptToRecognizeWith:)

Asks the delegate if a gesture recognizer should attempt to recognize gestures for a particular event.

macOS 10.11+

``` source
@MainActor
optional func gestureRecognizer(
    _ gestureRecognizer: NSGestureRecognizer,
    shouldAttemptToRecognizeWith event: NSEvent
) -> Bool
```

## Parameters 

`gestureRecognizer`  

The gesture recognizer object that is interpreting events. This is the object with which the delegate is associated.

`event`  

An event object associated with the request.

## Return Value

true to allow the gesture recognizer to begin recognizing gestures for the specified event, or false to prevent it from recognizing gestures for the specified event. If you do not implement this method, the default return value is true.

## Discussion

This method is called when a target view recognizes a new gesture event stream. The target view calls this method to determine whether the gesture recognizer should process events for the stream, or opt out of them. Returning false from this method causes the gesture recognizer to opt out, and prevents the other delegate methods from being called for the event stream.

## See Also

### Regulating Gesture Recognition

func gestureRecognizerShouldBegin(NSGestureRecognizer) -> Bool

Asks the delegate if a gesture recognizer should transition out of the Possible (`NSGestureRecognizerStatePossible`) state.

