

- AppKit
- NSGestureRecognizerDelegate
-  gestureRecognizer(\_:shouldRecognizeSimultaneouslyWith:) 

Instance Method

# gestureRecognizer(\_:shouldRecognizeSimultaneouslyWith:)

Asks the delegate if two gesture recognizers should be allowed to recognize their gestures simultaneously.

macOS 10.10+

``` source
@MainActor
optional func gestureRecognizer(
    _ gestureRecognizer: NSGestureRecognizer,
    shouldRecognizeSimultaneouslyWith otherGestureRecognizer: NSGestureRecognizer
) -> Bool
```

## Parameters 

`gestureRecognizer`  

The first gesture recognizer to be considered. This is the object with which the delegate is associated.

`otherGestureRecognizer`  

The second gesture recognizer to be considered.

## Return Value

true to allow `gestureRecognizer` and `otherGestureRecognizer` to recognize their gestures simultaneously. If you do not implement this method, the default return value is false—no two gestures can be recognized simultaneously.

## Discussion

This method is called when recognition of a gesture by either `gestureRecognizer` and `otherGestureRecognizer` would block the other gesture recognizer from recognizing its gesture. Returning true is guaranteed to allow simultaneous recognition; returning false is not guaranteed to prevent simultaneous recognition because the other gesture recognizer’s delegate may return true.

