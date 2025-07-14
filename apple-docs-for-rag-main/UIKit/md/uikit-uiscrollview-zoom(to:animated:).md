

- UIKit
- UIScrollView
-  zoom(to:animated:) 

Instance Method

# zoom(to:animated:)

Zooms to a specific area of the content so that it’s visible in the scroll view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func zoom(
    to rect: CGRect,
    animated: Bool
)
```

## Parameters 

`rect`  

A rectangle defining an area of the content view. The rectangle should be in the coordinate space of the view returned by viewForZooming(in:).

`animated`  

true if the scrolling should be animated, false if it should be immediate.

## Discussion

This method zooms so that the content view becomes the area defined by `rect`, adjusting the zoomScale as necessary.

## See Also

### Zooming and panning

var panGestureRecognizer: UIPanGestureRecognizer

The underlying gesture recognizer for pan gestures.

var pinchGestureRecognizer: UIPinchGestureRecognizer?

The underlying gesture recognizer for pinch gestures.

var zoomScale: CGFloat

A floating-point value that specifies the current scale factor applied to the scroll view’s content.

func setZoomScale(CGFloat, animated: Bool)

A floating-point value that specifies the current zoom scale.

var maximumZoomScale: CGFloat

A floating-point value that specifies the maximum scale factor that can apply to the scroll view’s content.

var minimumZoomScale: CGFloat

A floating-point value that specifies the minimum scale factor that can apply to the scroll view’s content.

var isZoomBouncing: Bool

A Boolean value that indicates that zooming has exceeded the scaling limits specified for the scroll view.

var isZooming: Bool

A Boolean value that indicates whether the content view is currently zooming in or out.

var isZoomAnimating: Bool

A Boolean value that indicates whether the scroll view is currently animating a zoom update.

var bouncesZoom: Bool

A Boolean value that determines whether the scroll view animates the content scaling when the scaling exceeds the maximum or minimum limits.

