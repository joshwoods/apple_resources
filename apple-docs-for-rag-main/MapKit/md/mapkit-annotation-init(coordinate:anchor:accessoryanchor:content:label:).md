

- MapKit
- Annotation
-  init(coordinate:anchor:accessoryAnchor:content:label:) 

Initializer

# init(coordinate:anchor:accessoryAnchor:content:label:)

Creates an annotation that displays a view at a coordinate on the map.

MapKitSwiftUIiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    coordinate: CLLocationCoordinate2D,
    anchor: UnitPoint = .center,
    accessoryAnchor: UnitPoint,
    @ViewBuilder content: () -> Content,
    @ViewBuilder label: () -> Label
)
```

## Parameters 

`coordinate`  

The coordinate position of the annotation.

`anchor`  

A UnitPoint value that indicates how to position the content around the provided coordinate.

`accessoryAnchor`  

A UnitPoint value that indicates how to place accessories around the provided content.

`content`  

The view to place on the map.

`label`  

The label for the annotation, including a title, and optional subtitle.

## See Also

### Creating annotations

init(LocalizedStringKey, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, accessoryAnchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init&lt;S>(S, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, accessoryAnchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init(item: MKMapItem, anchor: UnitPoint, accessoryAnchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init(LocalizedStringKey, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init&lt;S>(S, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map using a title key, coordinate, anchor location, and view you provide.

init(coordinate: CLLocationCoordinate2D, anchor: UnitPoint, content: () -> Content, label: () -> Label)

Creates an annotation that displays a view on the map using coordinates, anchor location, view, and label you provide.

