

- UIKit
- UITouch
-  majorRadiusTolerance 

Instance Property

# majorRadiusTolerance

The tolerance (in points) of the touch’s radius.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var majorRadiusTolerance: CGFloat { get }
```

## Discussion

This value determines the accuracy of the value in the majorRadius property. Add this value to the radius to get the maximum touch radius. Subtract the value to get the minimum touch radius.

## See Also

### Getting the location of a touch

func location(in: UIView?) -> CGPoint

Returns the current location of the touch in the coordinate system of the given view.

func previousLocation(in: UIView?) -> CGPoint

Returns the previous location of the touch in the coordinate system of the given view.

var view: UIView?

The view to which touches are being delivered, if any.

var window: UIWindow?

The window in which the touch initially occurred.

var majorRadius: CGFloat

The radius (in points) of the touch.

func preciseLocation(in: UIView?) -> CGPoint

Returns a precise location for the touch, when available.

func precisePreviousLocation(in: UIView?) -> CGPoint

Returns a precise previous location for the touch, when available.

