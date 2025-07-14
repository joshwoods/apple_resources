

- MapKit
- MKMapView
-  convert(\_:toRectTo:) 

Instance Method

# convert(\_:toRectTo:)

Converts a map region to a rectangle in the specified view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func convert(
    _ region: MKCoordinateRegion,
    toRectTo view: UIView?
) -> CGRect
```

**macOS**

``` source
@MainActor
func convert(
    _ region: MKCoordinateRegion,
    toRectTo view: NSView?
) -> CGRect
```

## Parameters 

`region`  

The map region that you want to find the corresponding view rectangle for.

`view`  

The view where you want to locate the specified map region. If this parameter is `nil`, the method specifies the returned rectangle in the window’s coordinate system. If `view` isn’t `nil`, the rectangle belongs to the same window as the map view.

## Return Value

The rectangle corresponding to the specified map region.

## See Also

### Converting map coordinates

func convert(CLLocationCoordinate2D, toPointTo: UIView?) -> CGPoint

Converts a map coordinate to a point in the specified view.

func convert(CGPoint, toCoordinateFrom: UIView?) -> CLLocationCoordinate2D

Converts a point in the specified view’s coordinate system to a map coordinate.

func convert(CGRect, toRegionFrom: UIView?) -> MKCoordinateRegion

Converts a rectangle in the specified view’s coordinate system to a map region.

