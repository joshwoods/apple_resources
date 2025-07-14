

- MapKit
-  MapPolygon 

Structure

# MapPolygon

A closed polygon overlay.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct MapPolygon
```

## Overview

Use this view to create map polygons instances in the closure you provide to the `content` parameter in the Map initializers.

## Topics

### Creating a map polygon

init(coordinates: [CLLocationCoordinate2D])

Creates a polygon from a list of coordinates you provide.

init(points: [MKMapPoint])

Creates a polygon from a list of map points.

init(MKPolygon)

Creates a polygon from the polygon you provide.

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

struct MapPolyline

An open polygon overlay consisting of one or more connected line segments.

struct Marker

A balloon-shaped annotation that marks a map location.

struct UserAnnotation

Displays the person’s current location on the map.

