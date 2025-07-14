

- MapKit
-  MapReader 

Structure

# MapReader

A container view that defines its contents as a function of information about the first contained map.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
struct MapReader where Content : View
```

## Overview

The map reader’s content builder receives a MapProxy instance. You can use this instance to get the information you’ll need to convert between a MapCamera and a MKMapRect or MKCoordinateRegion.

## Topics

### Creating a map reader

init(content: (MapProxy) -> Content)

Creates an instance that allows view content to reference information about a contained map.

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Structures

struct DefaultUserAnnotationContent

A structure that represents the view to show at the user’s location on the map.

struct EmptyMapContent

A map content element that doesn’t contain any content.

struct MapProxy

A proxy for accessing sizing information about a given map view.

struct TupleMapContent

A view created from a Swift tuple of map content values.

struct MapSelectableContentView

