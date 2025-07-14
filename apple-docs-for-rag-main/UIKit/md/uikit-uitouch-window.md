

- UIKit
- UITouch
-  window 

Instance Property

# window

The window in which the touch initially occurred.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var window: UIWindow? { get }
```

## Discussion

The value of the property is the window in which the touch originally occurred. This window might not be the same window that currently contains the touch.

## See Also

### Getting the location of a touch

func location(in: UIView?) -> CGPoint

Returns the current location of the touch in the coordinate system of the given view.

func previousLocation(in: UIView?) -> CGPoint

Returns the previous location of the touch in the coordinate system of the given view.

var view: UIView?

The view to which touches are being delivered, if any.

var majorRadius: CGFloat

The radius (in points) of the touch.

var majorRadiusTolerance: CGFloat

The tolerance (in points) of the touch’s radius.

func preciseLocation(in: UIView?) -> CGPoint

Returns a precise location for the touch, when available.

func precisePreviousLocation(in: UIView?) -> CGPoint

Returns a precise previous location for the touch, when available.

