

- MapKit
-  Marker 

Structure

# Marker

A balloon-shaped annotation that marks a map location.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
struct Marker where Label : View
```

## Overview

Use this view to create marker instances in the closure you provide to the `content` parameter in the Map initializers.

## Topics

### Creating a marker

init&lt;S>(S, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the label you provide.

init&lt;S>(S, image: String, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the provided title and image resource to display as the balloon’s icon.

init&lt;S>(S, systemImage: String, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the provided title and a system image the map displays as the balloon’s icon.

init(LocalizedStringKey, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the localized string key you provide.

init(LocalizedStringKey, image: String, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the provided localized title and image resource to display as the balloon’s icon.

init(LocalizedStringKey, monogram: Text, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the provided title key and monogram.

init&lt;S>(S, monogram: Text, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the provided title string and monogram.

init(LocalizedStringKey, systemImage: String, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with a localized title, and a system image the map displays as the balloon’s icon.

init(coordinate: CLLocationCoordinate2D, label: () -> Label)

Creates a marker at the given location with the provided label.

init(item: MKMapItem)

Creates a marker for a given map item using a MapKit-provided label.

### Displaying place information

func mapItemDetailSelectionAccessory(MapItemDetailSelectionAccessoryStyle?) -> some MapContent

Specifies the selection accessory to display for the selected map item content.

## Relationships

### Conforms To

- MapContent
- Sendable

## See Also

### Annotations and overlays

struct Annotation

A customizable annotation used to indicate a location on a map.

struct MapCircle

A circular overlay with a configurable radius that you center on a geographic coordinate.

struct MapPolygon

A closed polygon overlay.

struct MapPolyline

An open polygon overlay consisting of one or more connected line segments.

struct UserAnnotation

Displays the person’s current location on the map.

