

- UIKit
- UIScrollView
-  touchesShouldCancel(in:) 

Instance Method

# touchesShouldCancel(in:)

Returns whether to cancel touches related to the content subview and start dragging.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func touchesShouldCancel(in view: UIView) -> Bool
```

## Parameters 

`view`  

The view object in the content that’s being touched.

## Return Value

true to cancel further touch messages to `view`, false to have `view` continue to receive those messages. The default returned value is true if `view` is not a UIControl object; otherwise, it returns false.

## Discussion

The scroll view calls this method just after it starts sending tracking messages to the content view. If it receives false from this method, it stops dragging and forwards the touch events to the content subview. The scroll view doesn’t call this method if the value of the canCancelContentTouches property is false.

## See Also

### Managing touches

func touchesShouldBegin(Set&lt;UITouch>, with: UIEvent?, in: UIView) -> Bool

Overridden by subclasses to customize the default behavior when a finger touches down in displayed content.

var canCancelContentTouches: Bool

A Boolean value that controls whether touches in the content view always lead to tracking.

var delaysContentTouches: Bool

A Boolean value that determines whether the scroll view delays the handling of touch-down gestures.

var directionalPressGestureRecognizer: UIGestureRecognizer

The underlying gesture recognizer for directional button presses.

