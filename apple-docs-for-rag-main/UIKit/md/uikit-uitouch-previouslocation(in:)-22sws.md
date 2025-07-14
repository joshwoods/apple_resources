

- UIKit
- UITouch
-  previousLocation(in:) 

Instance Method

# previousLocation(in:)

Returns the previous location of the touch in the coordinate system of the given view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func previousLocation(in view: UIView?) -> CGPoint
```

## Parameters 

`view`  

The view object in whose coordinate system you want the touch located. A custom view that is handling the touch may specify `self` to get the touch location in its own coordinate system. Pass `nil` to get the touch location in the window’s coordinates.

## Return Value

This method returns the previous location of a UITouch object in the coordinate system of the specified view. Because the touch object might have been forwarded to a view from another view, this method performs any necessary conversion of the touch location to the coordinate system of the specified view.

## See Also

### Getting the location of a touch

func location(in: UIView?) -> CGPoint

Returns the current location of the touch in the coordinate system of the given view.

var view: UIView?

The view to which touches are being delivered, if any.

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

