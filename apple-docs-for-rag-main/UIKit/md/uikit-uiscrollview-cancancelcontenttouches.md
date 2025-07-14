

- UIKit
- UIScrollView
-  canCancelContentTouches 

Instance Property

# canCancelContentTouches

A Boolean value that controls whether touches in the content view always lead to tracking.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var canCancelContentTouches: Bool { get set }
```

## Discussion

If the value of this property is true and a view in the content has begun tracking a finger touching it, and if the user drags the finger enough to initiate a scroll, the view receives a touchesCancelled(_:with:) message and the scroll view handles the touch as a scroll. If the value of this property is false, the scroll view doesn’t scroll regardless of finger movement once the content view starts tracking.

## See Also

### Managing touches

func touchesShouldBegin(Set&lt;UITouch>, with: UIEvent?, in: UIView) -> Bool

Overridden by subclasses to customize the default behavior when a finger touches down in displayed content.

func touchesShouldCancel(in: UIView) -> Bool

Returns whether to cancel touches related to the content subview and start dragging.

var delaysContentTouches: Bool

A Boolean value that determines whether the scroll view delays the handling of touch-down gestures.

var directionalPressGestureRecognizer: UIGestureRecognizer

The underlying gesture recognizer for directional button presses.

