

- UIKit
- UIScrollView
-  isDragging 

Instance Property

# isDragging

A Boolean value that indicates whether the user has begun scrolling the content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isDragging: Bool { get }
```

## Discussion

The value held by this property might require some time or distance of scrolling before it returns true.

## See Also

### Managing the scrolling state

var isTracking: Bool

A Boolean value that indicates whether the user has touched the content to initiate scrolling.

var isDecelerating: Bool

A Boolean value that indicates whether the content is moving in the scroll view after the user lifted their finger.

var isScrollAnimating: Bool

A Boolean value that indicates whether the scroll view is currently animating a scroll update.

func stopScrollingAndZooming()

Stops active scroll and zoom animations.

var decelerationRate: UIScrollView.DecelerationRate

A floating-point value that determines the rate of deceleration after the user lifts their finger.

struct DecelerationRate

Deceleration rates for the scroll view.

