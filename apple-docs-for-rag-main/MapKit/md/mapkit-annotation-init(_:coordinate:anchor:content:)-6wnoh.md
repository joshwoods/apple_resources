

- MapKit
- Annotation
-  init(\_:coordinate:anchor:content:) 

Initializer

# init(\_:coordinate:anchor:content:)

Creates an annotation that displays a view at a coordinate on the map using a title key, coordinate, anchor location, and view you provide.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    _ title: S,
    coordinate: CLLocationCoordinate2D,
    anchor: UnitPoint = .center,
    @ViewBuilder content: () -> Content
) where Label == Text, S : StringProtocol
```

## Parameters 

`title`  

The title of the annotation.

`coordinate`  

The coordinate position of the annotation.

`anchor`  

A UnitPoint value that indicates how to position the content around the provided coordinate.

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

init(item: MKMapItem, anchor: UnitPoint, accessoryAnchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init(LocalizedStringKey, coordinate: CLLocationCoordinate2D, anchor: UnitPoint, content: () -> Content)

Creates an annotation that displays a view at a coordinate on the map.

init(coordinate: CLLocationCoordinate2D, anchor: UnitPoint, content: () -> Content, label: () -> Label)

Creates an annotation that displays a view on the map using coordinates, anchor location, view, and label you provide.

