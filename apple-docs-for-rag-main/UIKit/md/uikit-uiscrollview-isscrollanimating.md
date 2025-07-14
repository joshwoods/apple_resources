

- UIKit
- UIScrollView
-  isScrollAnimating 

Instance Property

# isScrollAnimating

A Boolean value that indicates whether the scroll view is currently animating a scroll update.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
var isScrollAnimating: Bool { get }
```

## Discussion

Call stopScrollingAndZooming() to stop the animation.

## See Also

### Managing the scrolling state

var isTracking: Bool

A Boolean value that indicates whether the user has touched the content to initiate scrolling.

var isDragging: Bool

A Boolean value that indicates whether the user has begun scrolling the content.

var isDecelerating: Bool

A Boolean value that indicates whether the content is moving in the scroll view after the user lifted their finger.

func stopScrollingAndZooming()

Stops active scroll and zoom animations.

var decelerationRate: UIScrollView.DecelerationRate

A floating-point value that determines the rate of deceleration after the user lifts their finger.

struct DecelerationRate

Deceleration rates for the scroll view.

