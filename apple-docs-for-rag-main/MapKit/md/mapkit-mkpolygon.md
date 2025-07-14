

- MapKit
-  MKPolygon 

Class

# MKPolygon

A closed polygon overlay.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKPolygon
```

## Overview

The points you add to this overlay connect end-to-end in the order you provide them. The first and last points connect to each other to create a closed shape.

When creating a polygon, you can mask out portions of the polygon by specifying one or more interior polygons. For the polygons you specify, this class uses the even-odd fill rule to determine the final occupied area. When applied to overlapping polygons, this rule can cause the framework to mask specific regions out and thereby remove them from the total occupied area. For more information about how fill rules apply to paths, see Paths in Quartz 2D Programming Guide.

## Topics

### Creating a polygon overlay

convenience init(points: UnsafePointer&lt;MKMapPoint>, count: Int)

Creates and returns a polygon object from the specified set of map points.

convenience init(points: UnsafePointer&lt;MKMapPoint>, count: Int, interiorPolygons: [MKPolygon]?)

Creates and returns a polygon object from the specified set of map points and interior polygons.

convenience init(coordinates: UnsafePointer&lt;CLLocationCoordinate2D>, count: Int)

Creates and returns a polygon object from the specified set of coordinates.

convenience init(coordinates: UnsafePointer&lt;CLLocationCoordinate2D>, count: Int, interiorPolygons: [MKPolygon]?)

Creates and returns a polygon object from the specified set of coordinates and interior polygons.

### Accessing the interior polygons

var interiorPolygons: [MKPolygon]?

The array of polygons that nest inside the enclosing polygon.

## Relationships

### Inherits From

- MKMultiPoint

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKAnnotation
- MKGeoJSONObject
- MKOverlay
- NSObjectProtocol

## See Also

### Custom shape overlays

class MKPolygonRenderer

The visual representation of a single polygon overlay.

class MKMultiPolygon

A collection of multiple closed polygon overlays.

class MKMultiPolygonRenderer

The visual representation of multiple polygon overlays.

class MKOverlayPathRenderer

The visual representation of a path-based overlay.

