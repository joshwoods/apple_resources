

- UIKit
- UIGestureRecognizer
-  require(toFail:) 

Instance Method

# require(toFail:)

Creates a dependency relationship between the gesture recognizer and another gesture recognizer when the objects are created.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func require(toFail otherGestureRecognizer: UIGestureRecognizer)
```

## Parameters 

`otherGestureRecognizer`  

Another gesture-recognizer object (an instance of a subclass of UIGestureRecognizer).

## Discussion

This method works fine when gesture recognizers aren’t created elsewhere in the app — or in a framework — and the set of gesture recognizers remains the same. If you need to set up failure requirements lazily or in different view hierarchies, use gestureRecognizer(_:shouldRequireFailureOf:) and gestureRecognizer(_:shouldBeRequiredToFailBy:) instead. (Note that the shouldRequireFailure(of:) and shouldBeRequiredToFail(by:) methods let subclasses define class-wide failure requirements.)

This method creates a relationship with another gesture recognizer that delays the current gesture recognizer’s transition out of UIGestureRecognizer.State.possible. The state that the current gesture recognizer transitions to depends on what happens with `otherGestureRecognizer`:

- If `otherGestureRecognizer` transitions to UIGestureRecognizer.State.failed, the current gesture recognizer transitions to its normal next state.

- If `otherGestureRecognizer` transitions to recognized or UIGestureRecognizer.State.began, the current gesture recognizer transitions to UIGestureRecognizer.State.failed.

An example where this method might be called is when you want a single-tap gesture require that a double-tap gesture fail.

## See Also

### Related Documentation

func shouldBeRequiredToFail(by: UIGestureRecognizer) -> Bool

Overridden to indicate that the receiver should be required to fail by the specified gesture recognizer.

func shouldRequireFailure(of: UIGestureRecognizer) -> Bool

Overridden to indicate that the receiver requires the specified gesture recognizer to fail.

