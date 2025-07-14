

- MapKit
- MKMapView
-  convert(\_:toPointTo:) 

Instance Method

# convert(\_:toPointTo:)

Converts a map coordinate to a point in the specified view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

**macOS**

``` source
@MainActor
func convert(
    _ coordinate: CLLocationCoordinate2D,
    toPointTo view: NSView?
) -> CGPoint
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func convert(
    _ coordinate: CLLocationCoordinate2D,
    toPointTo view: UIView?
) -> CGPoint
```

## Parameters 

`coordinate`  

The map coordinate that you want to find the corresponding point for.

`view`  

The view where you want to locate the specified map coordinate. If this parameter is `nil`, the method specifies the returned point in the window’s coordinate system. If `view` isn’t `nil`, the point belongs to the same window as the map view.

## Return Value

The point (in the appropriate view or window coordinate system) corresponding to the specified latitude and longitude value.

## See Also

### Converting map coordinates

func convert(CGPoint, toCoordinateFrom: UIView?) -> CLLocationCoordinate2D

Converts a point in the specified view’s coordinate system to a map coordinate.

func convert(MKCoordinateRegion, toRectTo: UIView?) -> CGRect

Converts a map region to a rectangle in the specified view.

func convert(CGRect, toRegionFrom: UIView?) -> MKCoordinateRegion

Converts a rectangle in the specified view’s coordinate system to a map region.

