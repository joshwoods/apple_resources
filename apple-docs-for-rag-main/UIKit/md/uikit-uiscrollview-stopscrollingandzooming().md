

- UIKit
- UIScrollView
-  stopScrollingAndZooming() 

Instance Method

# stopScrollingAndZooming()

Stops active scroll and zoom animations.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func stopScrollingAndZooming()
```

## Discussion

The scroll view’s content offset remains at the value it has when you call this method, unless:

- The scroll view is bouncing, in which case the content offset returns to the edge of the document.

- The scroll view is paging its content, in which case the content offset updates to a page boundary.

## See Also

### Managing the scrolling state

var isTracking: Bool

A Boolean value that indicates whether the user has touched the content to initiate scrolling.

var isDragging: Bool

A Boolean value that indicates whether the user has begun scrolling the content.

var isDecelerating: Bool

A Boolean value that indicates whether the content is moving in the scroll view after the user lifted their finger.

var isScrollAnimating: Bool

A Boolean value that indicates whether the scroll view is currently animating a scroll update.

var decelerationRate: UIScrollView.DecelerationRate

A floating-point value that determines the rate of deceleration after the user lifts their finger.

struct DecelerationRate

Deceleration rates for the scroll view.

