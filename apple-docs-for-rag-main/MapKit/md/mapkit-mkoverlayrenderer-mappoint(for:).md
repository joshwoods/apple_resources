

- MapKit
- MKOverlayRenderer
-  mapPoint(for:) 

Instance Method

# mapPoint(for:)

Returns the point on the map that corresponds to the specified point in the overlay renderer’s drawing area.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func mapPoint(for point: CGPoint) -> MKMapPoint
```

## Parameters 

`point`  

The point in the overlay’s drawing area that you want to convert.

## Return Value

The point on the two-dimensional map projection corresponding to the specified point.

## Discussion

You may call this method safely from your view’s draw(_:zoomScale:in:) method.

## See Also

### Converting points on the map

func point(for: MKMapPoint) -> CGPoint

Returns the point in the overlay renderer’s drawing area corresponding to the specified point on the map.

func rect(for: MKMapRect) -> CGRect

Returns the rectangle in the overlay renderer’s drawing area corresponding to the specified rectangle on the map.

func mapRect(for: CGRect) -> MKMapRect

Returns the rectangle on the map that corresponds to the specified rectangle in the overlay renderer’s drawing area.

