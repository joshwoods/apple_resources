

- MapKit
- MKOverlayRenderer
-  canDraw(\_:zoomScale:) 

Instance Method

# canDraw(\_:zoomScale:)

Returns a Boolean value that indicates whether the overlay view is ready to draw its content.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func canDraw(
    _ mapRect: MKMapRect,
    zoomScale: MKZoomScale
) -> Bool
```

## Parameters 

`mapRect`  

The map rectangle that the renderer needs to update.

`zoomScale`  

The current scale factor applied to the map.

## Return Value

true if this overlay renderer is ready to draw its contents on the map or false if it is not.

## Discussion

Overlay renderers can override this method in situations where they may depend on the availability of other information to draw their contents. For example, a renderer showing traffic information might want to delay drawing until it has all of the traffic data it needs. In such a case, it can return false from this method to indicate that it’s not ready. An overlay renderer might also return false if it doesn’t draw content in the specified rectangle.

If you return false from this method, your application is responsible for calling the setNeedsDisplay(_:zoomScale:) method when the overlay renderer subsequently becomes ready to draw its contents.

The default implementation of this method returns true.

## See Also

### Drawing the overlay

func draw(MKMapRect, zoomScale: MKZoomScale, in: CGContext)

Draws the overlay’s contents at the specified location on the map.

func setNeedsDisplay()

Invalidates the entire contents of the overlay for all zoom scales.

func setNeedsDisplay(MKMapRect)

Invalidates the specified portion of the overlay at all zoom scales.

func setNeedsDisplay(MKMapRect, zoomScale: MKZoomScale)

Invalidates the specified portion of the overlay, but only at the specified zoom scale.

