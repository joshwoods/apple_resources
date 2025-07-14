

- MapKit
- MKMapView
-  convert(\_:toRegionFrom:) 

Instance Method

# convert(\_:toRegionFrom:)

Converts a rectangle in the specified view’s coordinate system to a map region.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func convert(
    _ rect: CGRect,
    toRegionFrom view: UIView?
) -> MKCoordinateRegion
```

**macOS**

``` source
@MainActor
func convert(
    _ rect: CGRect,
    toRegionFrom view: NSView?
) -> MKCoordinateRegion
```

## Parameters 

`rect`  

The rectangle you want to convert.

`view`  

The view that serves as the reference coordinate system for the `rect` parameter.

## Return Value

The map region corresponding to the specified view rectangle.

## See Also

### Converting map coordinates

func convert(CLLocationCoordinate2D, toPointTo: UIView?) -> CGPoint

Converts a map coordinate to a point in the specified view.

func convert(CGPoint, toCoordinateFrom: UIView?) -> CLLocationCoordinate2D

Converts a point in the specified view’s coordinate system to a map coordinate.

func convert(MKCoordinateRegion, toRectTo: UIView?) -> CGRect

Converts a map region to a rectangle in the specified view.

