

- UIKit
- UIScrollView
-  decelerationRate 

Instance Property

# decelerationRate

A floating-point value that determines the rate of deceleration after the user lifts their finger.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var decelerationRate: UIScrollView.DecelerationRate { get set }
```

## Discussion

The default rate is normal. For possible deceleration rates, see UIScrollView.DecelerationRate.

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

func stopScrollingAndZooming()

Stops active scroll and zoom animations.

struct DecelerationRate

Deceleration rates for the scroll view.

