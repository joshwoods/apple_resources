

- UIKit
- UIScrollView
-  directionalPressGestureRecognizer 

Instance Property

# directionalPressGestureRecognizer

The underlying gesture recognizer for directional button presses.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOS 9.0–11.0DeprecatedvisionOS 1.0+

``` source
@MainActor
var directionalPressGestureRecognizer: UIGestureRecognizer { get }
```

## Discussion

The directionalPressGestureRecognizer is disabled by default. If you want to perform scrolling in direct response to up, down, left, and right arrow button presses, instead of scrolling indirectly in response to focus updates, enable this gesture recognizer.

## See Also

### Managing touches

func touchesShouldBegin(Set&lt;UITouch>, with: UIEvent?, in: UIView) -> Bool

Overridden by subclasses to customize the default behavior when a finger touches down in displayed content.

func touchesShouldCancel(in: UIView) -> Bool

Returns whether to cancel touches related to the content subview and start dragging.

var canCancelContentTouches: Bool

A Boolean value that controls whether touches in the content view always lead to tracking.

var delaysContentTouches: Bool

A Boolean value that determines whether the scroll view delays the handling of touch-down gestures.

