

- MapKit
-  MapAnnotation Deprecated

Structure

# MapAnnotation

A customizable annotation that marks a map location.

MapKitSwiftUIiOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac CatalystmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedvisionOSwatchOS 7.0–10.0Deprecated

``` source
struct MapAnnotation where Content : View
```

Deprecated

Use Annotation along with Map initializers that take a MapContentBuilder instead.

## Overview

Use MapAnnotation to declare the layout of the view that MapKit uses for the annotation. Create a Map and display annotations by returning a view that conforms to MapAnnotationProtocol from the trailing closure of init(coordinateRegion:interactionModes:showsUserLocation:userTrackingMode:annotationItems:annotationContent:) or init(mapRect:interactionModes:showsUserLocation:userTrackingMode:annotationItems:annotationContent:). Items you provide as a collection to the source annotations need to conform to Identifiable.

For example, the following code displays a map and a single annotation:

```
struct IdentifiablePlace: Identifiable {
    let id: UUID
    let location: CLLocationCoordinate2D
    init(id: UUID = UUID(), lat: Double, long: Double) {
        self.id = id
        self.location = CLLocationCoordinate2D(
            latitude: lat,
            longitude: long)
    }
}

struct CustomAnnotationMapView: View {
    let place: IdentifiablePlace
    @State var region: MKCoordinateRegion

    var body: some View {
        Map(coordinateRegion: $region,
            annotationItems: [place]
        ) { place in
            MapAnnotation(coordinate: place.location) {
                Rectangle().stroke(Color.blue)
                .frame(width: 20, height: 20)
            }
        }
    }
}
```

## Topics

### Creating a map annotation

init(coordinate: CLLocationCoordinate2D, anchorPoint: CGPoint, content: () -> Content)

Creates a custom annotation that provides a SwiftUI view to display at the map location that you specify.

## Relationships

### Conforms To

- MapAnnotationProtocol

## See Also

### Structures

struct MapMarker

A balloon-shaped annotation used to indicate the location on a map.

Deprecated

struct MapPin

A pin-shaped annotation used to indicate a location on a map.

Deprecated

