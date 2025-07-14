

- MapKit
- MapPolyline
-  init(coordinates:contourStyle:) 

Initializer

# init(coordinates:contourStyle:)

Creates a polyline that traces a path between the given coordinates using the specifed contour style.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
init(
    coordinates: [CLLocationCoordinate2D],
    contourStyle: MapPolyline.ContourStyle = .straight
)
```

## Parameters 

`coordinates`  

The coordinates to trace the path between.

`contourStyle`  

The MapPolyline.ContourStyle to use.

## See Also

### Creating a polyline

init(MKPolyline)

Creates a polyline from polyline you provide.

init(MKRoute)

Creates a polyline that traces the route you provide.

init(points: [MKMapPoint], contourStyle: MapPolyline.ContourStyle)

Creates a new polyline that traces a path between the provided points using the specifed contour style.

