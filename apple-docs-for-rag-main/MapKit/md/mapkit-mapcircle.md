

- MapKit
-  MapCircle 

Structure

# MapCircle

A circular overlay with a configurable radius that you center on a geographic coordinate.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct MapCircle
```

## Overview

Use this view to create circular overlays in the closure you provide to the `content` parameter in Map initializers.

## Topics

### Creating a map circle

init(MKCircle)

Creates a circle overlay from an existing map circle object.

init(center: CLLocationCoordinate2D, radius: CLLocationDistance)

Creates a circle with the center coordinate and radius you specify.

init(mapRect: MKMapRect)

Creates the largest possible circle centered within the given map rectangle.

## Relationships

### Conforms To

- Copyable
- MapContent

## See Also

### Annotations and overlays

struct Annotation

A customizable annotation used to indicate a location on a map.

struct MapPolygon

A closed polygon overlay.

struct MapPolyline

An open polygon overlay consisting of one or more connected line segments.

struct Marker

A balloon-shaped annotation that marks a map location.

struct UserAnnotation

Displays the person’s current location on the map.

