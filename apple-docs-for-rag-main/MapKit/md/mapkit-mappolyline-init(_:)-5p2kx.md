

- MapKit
- MapPolyline
-  init(\_:) 

Initializer

# init(\_:)

Creates a polyline that traces the route you provide.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS

``` source
init(_ route: MKRoute)
```

## Parameters 

`route`  

The MKRoute to trace.

## See Also

### Creating a polyline

init(MKPolyline)

Creates a polyline from polyline you provide.

init(coordinates: [CLLocationCoordinate2D], contourStyle: MapPolyline.ContourStyle)

Creates a polyline that traces a path between the given coordinates using the specifed contour style.

init(points: [MKMapPoint], contourStyle: MapPolyline.ContourStyle)

Creates a new polyline that traces a path between the provided points using the specifed contour style.

