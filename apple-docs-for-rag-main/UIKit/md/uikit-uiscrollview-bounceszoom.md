

- UIKit
- UIScrollView
-  bouncesZoom 

Instance Property

# bouncesZoom

A Boolean value that determines whether the scroll view animates the content scaling when the scaling exceeds the maximum or minimum limits.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var bouncesZoom: Bool { get set }
```

## Discussion

If the value of this property is true and zooming exceeds either the maximum or minimum limits for scaling, the scroll view temporarily animates the content scaling just past these limits before returning to them. If this property is false, zooming stops immediately at one a scaling limits. The default value is true.

## See Also

### Zooming and panning

var panGestureRecognizer: UIPanGestureRecognizer

The underlying gesture recognizer for pan gestures.

var pinchGestureRecognizer: UIPinchGestureRecognizer?

The underlying gesture recognizer for pinch gestures.

func zoom(to: CGRect, animated: Bool)

Zooms to a specific area of the content so that it’s visible in the scroll view.

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

