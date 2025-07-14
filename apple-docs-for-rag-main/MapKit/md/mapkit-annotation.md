

- MapKit
-  Annotation 

Structure

# Annotation

A customizable annotation used to indicate a location on a map.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
struct Annotation where Label : View, Content : View
```

## Overview

Use this view to annotations in the closure you provide to the `content` parameter in the Map initializers.

## Topics

### Creating annotations

init(LocalizedStringKey, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, accessoryAnchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init&lt;S>(S, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, accessoryAnchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init(coordinate: CLLocationCoordinate2D, anchor: UnitPoint, accessoryAnchor: UnitPoint, content: () -> Content, label: () -> Label)

Creates an annotation that displays a view at a coordinate on the map.

init(item: MKMapItem, anchor: UnitPoint, accessoryAnchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init(LocalizedStringKey, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init&lt;S>(S, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map using a title key, coordinate, anchor location, and view you provide.

init(coordinate: CLLocationCoordinate2D, anchor: UnitPoint, content: () -> Content, label: () -> Label)

Creates an annotation that displays a view on the map using coordinates, anchor location, view, and label you provide.

### Displaying place information

func mapItemDetailSelectionAccessory(MapItemDetailSelectionAccessoryStyle?) -> some MapContent

Specifies the selection accessory to display for the selected map item content.

## Relationships

### Conforms To

- MapContent
- Sendable

## See Also

### Annotations and overlays

struct MapCircle

A circular overlay with a configurable radius that you center on a geographic coordinate.

struct MapPolygon

A closed polygon overlay.

struct MapPolyline

An open polygon overlay consisting of one or more connected line segments.

struct Marker

A balloon-shaped annotation that marks a map location.

struct UserAnnotation

Displays the person’s current location on the map.

