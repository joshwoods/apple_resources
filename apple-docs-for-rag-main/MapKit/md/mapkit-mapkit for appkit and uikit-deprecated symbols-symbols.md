

- MapKit
- MapKit for AppKit and UIKit
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Map protocols and view modifiers that are no longer supported.

## Topics

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

init&lt;Items, Annotation>(mapRect: Binding&lt;MKMapRect>, interactionModes: MapInteractionModes, showsUserLocation: Bool, userTrackingMode: Binding&lt;MapUserTrackingMode>?, annotationItems: Items, annotationContent: (Items.Element) -> Annotation)

Creates a map that displays a map rectangle with annotations, and optionally configures available interactions, user location, and tracking behavior.

Deprecated

### Structures

struct MapAnnotation

A customizable annotation that marks a map location.

Deprecated

struct MapMarker

A balloon-shaped annotation used to indicate the location on a map.

Deprecated

struct MapPin

A pin-shaped annotation used to indicate a location on a map.

Deprecated

### Enumerations

enum MapUserTrackingMode

The modes available for user tracking.

Deprecated

