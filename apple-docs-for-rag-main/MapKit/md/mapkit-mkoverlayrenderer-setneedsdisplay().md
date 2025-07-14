

- MapKit
- MKOverlayRenderer
-  setNeedsDisplay() 

Instance Method

# setNeedsDisplay()

Invalidates the entire contents of the overlay for all zoom scales.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func setNeedsDisplay()
```

## Discussion

This method causes the entire contents of the overlay to be redrawn during the next update cycle. This method invalidates the overlay regardless of the current zoom scale associated with the map.

## See Also

### Drawing the overlay

func canDraw(MKMapRect, zoomScale: MKZoomScale) -> Bool

Returns a Boolean value that indicates whether the overlay view is ready to draw its content.

func draw(MKMapRect, zoomScale: MKZoomScale, in: CGContext)

Draws the overlay’s contents at the specified location on the map.

func setNeedsDisplay(MKMapRect)

Invalidates the specified portion of the overlay at all zoom scales.

func setNeedsDisplay(MKMapRect, zoomScale: MKZoomScale)

Invalidates the specified portion of the overlay, but only at the specified zoom scale.

