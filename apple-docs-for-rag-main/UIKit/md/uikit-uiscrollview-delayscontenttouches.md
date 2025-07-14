

- UIKit
- UIScrollView
-  delaysContentTouches 

Instance Property

# delaysContentTouches

A Boolean value that determines whether the scroll view delays the handling of touch-down gestures.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var delaysContentTouches: Bool { get set }
```

## Discussion

If the value of this property is true, the scroll view delays handling the touch-down gesture until it can determine if scrolling is the intent. If the value is false , the scroll view immediately calls touchesShouldBegin(_:with:in:). The default value is true.

See the class description for a fuller discussion.

## See Also

### Managing touches

func touchesShouldBegin(Set&lt;UITouch>, with: UIEvent?, in: UIView) -> Bool

Overridden by subclasses to customize the default behavior when a finger touches down in displayed content.

func touchesShouldCancel(in: UIView) -> Bool

Returns whether to cancel touches related to the content subview and start dragging.

var canCancelContentTouches: Bool

A Boolean value that controls whether touches in the content view always lead to tracking.

var directionalPressGestureRecognizer: UIGestureRecognizer

The underlying gesture recognizer for directional button presses.

