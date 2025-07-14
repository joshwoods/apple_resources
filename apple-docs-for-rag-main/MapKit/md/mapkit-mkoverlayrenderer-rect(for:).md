

- MapKit
- MKOverlayRenderer
-  rect(for:) 

Instance Method

# rect(for:)

Returns the rectangle in the overlay renderer’s drawing area corresponding to the specified rectangle on the map.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func rect(for mapRect: MKMapRect) -> CGRect
```

## Parameters 

`mapRect`  

A rectangle on the two-dimensional map projection.

## Return Value

The rectangle in the overlay’s drawing area that corresponds to the map rectangle.

## Discussion

You may call this method safely from your view’s draw(_:zoomScale:in:) method.

## See Also

### Converting points on the map

func point(for: MKMapPoint) -> CGPoint

Returns the point in the overlay renderer’s drawing area corresponding to the specified point on the map.

func mapPoint(for: CGPoint) -> MKMapPoint

Returns the point on the map that corresponds to the specified point in the overlay renderer’s drawing area.

func mapRect(for: CGRect) -> MKMapRect

Returns the rectangle on the map that corresponds to the specified rectangle in the overlay renderer’s drawing area.

