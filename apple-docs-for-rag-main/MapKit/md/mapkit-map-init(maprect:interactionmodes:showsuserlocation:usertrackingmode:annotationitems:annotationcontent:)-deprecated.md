

- MapKit
- Map
-  init(mapRect:interactionModes:showsUserLocation:userTrackingMode:annotationItems:annotationContent:) Deprecated

Initializer

# init(mapRect:interactionModes:showsUserLocation:userTrackingMode:annotationItems:annotationContent:)

Creates a map that displays a map rectangle with annotations, and optionally configures available interactions, user location, and tracking behavior.

MapKitSwiftUIiOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac CatalystmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedvisionOSwatchOS 7.0–10.0Deprecated

``` source
@MainActor @preconcurrency
init(
    mapRect: Binding,
    interactionModes: MapInteractionModes = .all,
    showsUserLocation: Bool = false,
    userTrackingMode: Binding? = nil,
    annotationItems: Items,
    annotationContent: @escaping (Items.Element) -> Annotation
) where Content == _DefaultAnnotatedMapContent, Items : RandomAccessCollection, Annotation : MapAnnotationProtocol, Items.Element : Identifiable
```

Deprecated

Use Map initializers that take a MapContentBuilder instead.

## Parameters 

`mapRect`  

The map rectangle defining the area to display.

`interactionModes`  

An enumeration that indicates the user interactions to which the map responds.

`showsUserLocation`  

A Boolean value that indicates the option to display a person’s location on a map. The map displays the location only if they authorized the app to access their location.

`userTrackingMode`  

A binding to a tracking mode that determines how the map responds to location updates.

`annotationItems`  

The collection of data that the view uses to display annotations.

`annotationContent`  

A closure that produces the annotation content.

## See Also

### Initializers

init(coordinateRegion: Binding&lt;MKCoordinateRegion>, interactionModes: MapInteractionModes, showsUserLocation: Bool, userTrackingMode: Binding&lt;MapUserTrackingMode>?)

Creates a map that displays a coordinate region and optionally configures available interactions, user location, and tracking behavior.

Deprecated

init&lt;Items, Annotation>(coordinateRegion: Binding&lt;MKCoordinateRegion>, interactionModes: MapInteractionModes, showsUserLocation: Bool, userTrackingMode: Binding&lt;MapUserTrackingMode>?, annotationItems: Items, annotationContent: (Items.Element) -> Annotation)

Creates a map that displays a coordinate region with annotations, and optionally configures available interactions, user location, and tracking behavior.

Deprecated

init(mapRect: Binding&lt;MKMapRect>, interactionModes: MapInteractionModes, showsUserLocation: Bool, userTrackingMode: Binding&lt;MapUserTrackingMode>?)

Creates a map that displays a map rectangle and optionally configures available interactions, user location, and tracking behavior.

Deprecated

