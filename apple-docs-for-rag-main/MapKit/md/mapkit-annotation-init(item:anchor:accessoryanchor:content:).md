

- MapKit
- Annotation
-  init(item:anchor:accessoryAnchor:content:) 

Initializer

# init(item:anchor:accessoryAnchor:content:)

Creates an annotation that displays a view at a coordinate on the map.

MapKitSwiftUIiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    item: MKMapItem,
    anchor: UnitPoint = .center,
    accessoryAnchor: UnitPoint = .center,
    @ViewBuilder content: () -> Content
) where Label == Text
```

## Parameters 

`item`  

A map item that provides a label and coordinate for the annotation.

`anchor`  

A UnitPoint value that indicates how to position the content around the provided coordinate.

`accessoryAnchor`  

A UnitPoint value that indicates how to place accessories around the provided content.

`content`  

The view to place on the map.

## See Also

### Creating annotations

init(LocalizedStringKey, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, accessoryAnchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init&lt;S>(S, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, accessoryAnchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init(coordinate: CLLocationCoordinate2D, anchor: UnitPoint, accessoryAnchor: UnitPoint, content: () -> Content, label: () -> Label)

Creates an annotation that displays a view at a coordinate on the map.

init(LocalizedStringKey, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init&lt;S>(S, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map using a title key, coordinate, anchor location, and view you provide.

init(coordinate: CLLocationCoordinate2D, anchor: UnitPoint, content: () -> Content, label: () -> Label)

Creates an annotation that displays a view on the map using coordinates, anchor location, view, and label you provide.

