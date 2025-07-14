

- UIKit
- UIScrollView
-  touchesShouldBegin(\_:with:in:) 

Instance Method

# touchesShouldBegin(\_:with:in:)

Overridden by subclasses to customize the default behavior when a finger touches down in displayed content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func touchesShouldBegin(
    _ touches: Set,
    with event: UIEvent?,
    in view: UIView
) -> Bool
```

## Parameters 

`touches`  

A set of UITouch instances that represent the touches for the starting phase of the event represented by `event`.

`event`  

An object representing the event to which the touch objects in `touches` belong.

`view`  

The subview in the content where the touch-down gesture occurred.

## Return Value

Return false if you don’t want the scroll view to send event messages to `view`. If you want `view` to receive those messages, return true (the default).

## Discussion

The default behavior of UIScrollView is to invoke the UIResponder event-handling methods of the target subview that the touches occur in.

## See Also

### Managing touches

func touchesShouldCancel(in: UIView) -> Bool

Returns whether to cancel touches related to the content subview and start dragging.

var canCancelContentTouches: Bool

A Boolean value that controls whether touches in the content view always lead to tracking.

var delaysContentTouches: Bool

A Boolean value that determines whether the scroll view delays the handling of touch-down gestures.

var directionalPressGestureRecognizer: UIGestureRecognizer

The underlying gesture recognizer for directional button presses.

