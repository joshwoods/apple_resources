

- MapKit
- MKMapView
-  convert(\_:toCoordinateFrom:) 

Instance Method

# convert(\_:toCoordinateFrom:)

Converts a point in the specified view’s coordinate system to a map coordinate.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func convert(
    _ point: CGPoint,
    toCoordinateFrom view: UIView?
) -> CLLocationCoordinate2D
```

**macOS**

``` source
@MainActor
func convert(
    _ point: CGPoint,
    toCoordinateFrom view: NSView?
) -> CLLocationCoordinate2D
```

## Parameters 

`point`  

The point you want to convert.

`view`  

The view that serves as the reference coordinate system for the `point` parameter.

## Return Value

The map coordinate at the specified point.

## See Also

### Converting map coordinates

func convert(CLLocationCoordinate2D, toPointTo: UIView?) -> CGPoint

Converts a map coordinate to a point in the specified view.

func convert(MKCoordinateRegion, toRectTo: UIView?) -> CGRect

Converts a map region to a rectangle in the specified view.

func convert(CGRect, toRegionFrom: UIView?) -> MKCoordinateRegion

Converts a rectangle in the specified view’s coordinate system to a map region.

