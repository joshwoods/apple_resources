

- UIKit
- UITouch
-  preciseLocation(in:) 

Instance Method

# preciseLocation(in:)

Returns a precise location for the touch, when available.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func preciseLocation(in view: UIView?) -> CGPoint
```

## Parameters 

`view`  

The view that contains the touch.

## Return Value

A precise location for the touch.

## Mentioned in 

Implementing coalesced touch support in an app

## Discussion

Use this method to get additional precision for a touch (when available). Do not use the returned point for hit testing. In some cases, hit testing can indicate that the touch is within a view, but hit testing against the more precise location may indicate that the touch is outside of the view.

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

var majorRadiusTolerance: CGFloat

The tolerance (in points) of the touch’s radius.

func precisePreviousLocation(in: UIView?) -> CGPoint

Returns a precise previous location for the touch, when available.

