

- MapKit
-  MapPolyline 

Structure

# MapPolyline

An open polygon overlay consisting of one or more connected line segments.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct MapPolyline
```

## Overview

Use this view to create map polylines instances in the closure you provide to the `content` parameter in the Map initializers.

## Topics

### Creating a polyline

init(MKPolyline)

Creates a polyline from polyline you provide.

init(MKRoute)

Creates a polyline that traces the route you provide.

init(coordinates: [CLLocationCoordinate2D], contourStyle: MapPolyline.ContourStyle)

Creates a polyline that traces a path between the given coordinates using the specifed contour style.

init(points: [MKMapPoint], contourStyle: MapPolyline.ContourStyle)

Creates a new polyline that traces a path between the provided points using the specifed contour style.

### Styling the polyline

struct ContourStyle

Values that define how MapKit styles lines to represent the contour of the Earth.

## Relationships

### Conforms To

- Copyable
- MapContent

## See Also

### Annotations and overlays

struct Annotation

A customizable annotation used to indicate a location on a map.

struct MapCircle

A circular overlay with a configurable radius that you center on a geographic coordinate.

struct MapPolygon

A closed polygon overlay.

struct Marker

A balloon-shaped annotation that marks a map location.

struct UserAnnotation

Displays the person’s current location on the map.

