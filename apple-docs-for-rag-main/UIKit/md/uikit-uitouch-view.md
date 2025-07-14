

- UIKit
- UITouch
-  view 

Instance Property

# view

The view to which touches are being delivered, if any.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var view: UIView? { get }
```

## Mentioned in 

Using responders and the responder chain to handle events

## Discussion

The value of this property is the view object to which touches are being delivered, which is not necessarily the view the touch is currently in. For example, when a gesture recognizer recognizes the touch, this property is `nil` because no view is receiving the touch.

## See Also

### Getting the location of a touch

func location(in: UIView?) -> CGPoint

Returns the current location of the touch in the coordinate system of the given view.

func previousLocation(in: UIView?) -> CGPoint

Returns the previous location of the touch in the coordinate system of the given view.

var window: UIWindow?

The window in which the touch initially occurred.

var majorRadius: CGFloat

The radius (in points) of the touch.

var majorRadiusTolerance: CGFloat

The tolerance (in points) of the touch’s radius.

func preciseLocation(in: UIView?) -> CGPoint

Returns a precise location for the touch, when available.

func precisePreviousLocation(in: UIView?) -> CGPoint

Returns a precise previous location for the touch, when available.

