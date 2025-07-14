

- UIKit
- UIScrollView
-  isDecelerating 

Instance Property

# isDecelerating

A Boolean value that indicates whether the content is moving in the scroll view after the user lifted their finger.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isDecelerating: Bool { get }
```

## Discussion

The returned value is true if user isn’t dragging the content but scrolling is still occurring.

## See Also

### Managing the scrolling state

var isTracking: Bool

A Boolean value that indicates whether the user has touched the content to initiate scrolling.

var isDragging: Bool

A Boolean value that indicates whether the user has begun scrolling the content.

var isScrollAnimating: Bool

A Boolean value that indicates whether the scroll view is currently animating a scroll update.

func stopScrollingAndZooming()

Stops active scroll and zoom animations.

var decelerationRate: UIScrollView.DecelerationRate

A floating-point value that determines the rate of deceleration after the user lifts their finger.

struct DecelerationRate

Deceleration rates for the scroll view.

