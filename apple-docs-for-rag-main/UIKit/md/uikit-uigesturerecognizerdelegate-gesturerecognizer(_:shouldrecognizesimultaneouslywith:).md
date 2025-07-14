

- UIKit
- UIGestureRecognizerDelegate
-  gestureRecognizer(\_:shouldRecognizeSimultaneouslyWith:) 

Instance Method

# gestureRecognizer(\_:shouldRecognizeSimultaneouslyWith:)

Asks the delegate if two gesture recognizers should be allowed to recognize gestures simultaneously.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func gestureRecognizer(
    _ gestureRecognizer: UIGestureRecognizer,
    shouldRecognizeSimultaneouslyWith otherGestureRecognizer: UIGestureRecognizer
) -> Bool
```

## Parameters 

`gestureRecognizer`  

An instance of a subclass of the abstract base class UIGestureRecognizer. This is the object sending the message to the delegate.

`otherGestureRecognizer`  

An instance of a subclass of the abstract base class UIGestureRecognizer.

## Return Value

true to allow both `gestureRecognizer` and `otherGestureRecognizer` to recognize their gestures simultaneously. The default implementation returns false—no two gestures can be recognized simultaneously.

## Mentioned in 

Allowing the simultaneous recognition of multiple gestures

## Discussion

This method is called when recognition of a gesture by either `gestureRecognizer` or `otherGestureRecognizer` would block the other gesture recognizer from recognizing its gesture. Note that returning true is guaranteed to allow simultaneous recognition; returning false, on the other hand, is not guaranteed to prevent simultaneous recognition because the other gesture recognizer’s delegate may return true.

