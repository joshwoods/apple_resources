

- AppKit
- NSGestureRecognizerDelegate
-  gestureRecognizer(\_:shouldRequireFailureOf:) 

Instance Method

# gestureRecognizer(\_:shouldRequireFailureOf:)

Asks the delegate if the current gesture recognizer must wait to recognize its gesture until the specified gesture recognizer fails.

macOS 10.10+

``` source
@MainActor
optional func gestureRecognizer(
    _ gestureRecognizer: NSGestureRecognizer,
    shouldRequireFailureOf otherGestureRecognizer: NSGestureRecognizer
) -> Bool
```

## Parameters 

`gestureRecognizer`  

The gesture recognizer that might need to wait to recognize its gesture. This is the object with which the delegate is associated.

`otherGestureRecognizer`  

The gesture recognizer that must fail before the object in `gestureRecognizer` can recognize its gesture.

## Return Value

true if `otherGestureRecognizer` must fail before `gestureRecognizer` is allowed to recognize its gesture. If you do not implement this method, the default return value is false.

## Discussion

This method is called once per attempt to recognize, so you can change the failure requirements dynamically. The two gesture recognizers do not have to belong to the same view hierarchy.

Returning true is guaranteed to set up the failure requirement; returning false does not prevent the failure requirement from being set up by the other gesture recognizer.

## See Also

### Setting Up Failure Requirements

func gestureRecognizer(NSGestureRecognizer, shouldBeRequiredToFailBy: NSGestureRecognizer) -> Bool

Asks the delegate if the current gesture recognizer must fail before another gesture recognizer is allowed to recognize its gesture.

