

- UIKit
- UITouch
-  majorRadius 

Instance Property

# majorRadius

The radius (in points) of the touch.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var majorRadius: CGFloat { get }
```

## Discussion

Use the value in this property to determine the size of the touch that was reported by the hardware. This value is an approximation of the size and can vary by the amount specified in the majorRadiusTolerance property.

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

var majorRadiusTolerance: CGFloat

The tolerance (in points) of the touch’s radius.

func preciseLocation(in: UIView?) -> CGPoint

Returns a precise location for the touch, when available.

func precisePreviousLocation(in: UIView?) -> CGPoint

Returns a precise previous location for the touch, when available.

