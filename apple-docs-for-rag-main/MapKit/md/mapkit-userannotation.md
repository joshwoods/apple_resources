

- MapKit
-  UserAnnotation 

Structure

# UserAnnotation

Displays the person’s current location on the map.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
struct UserAnnotation where Content : View
```

## Overview

Displays the person’s current location using the system styled user location indicator.

## Topics

### Creating a user annotation

init()

Creates an annotation that displays the person’s current location.

init(anchor: UnitPoint)

Creates an annotation that displays the person’s current location using the system styled user location indicator with the specified anchor point.

init(anchor: UnitPoint, content: (UserLocation) -> Content)

Creates an annotation that displays a person’s current location using the system styled user location indicator with the specified anchor point using a custom view.

init(anchor: UnitPoint, content: () -> Content)

Create an annotation that displays the person’s current location of the user using a custom view.

### Information about a person’s location

struct UserLocation

A structure that contains Information about the person’s current location.

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

struct Marker

A balloon-shaped annotation that marks a map location.

