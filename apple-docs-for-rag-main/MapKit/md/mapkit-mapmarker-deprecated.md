

- MapKit
-  MapMarker Deprecated

Structure

# MapMarker

A balloon-shaped annotation used to indicate the location on a map.

MapKitSwiftUIiOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac CatalystmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedvisionOSwatchOS 7.0–10.0Deprecated

``` source
struct MapMarker
```

Deprecated

Use Marker along with Map initializers that take a MapContentBuilder instead.

## Overview

Create a Map and display marker annotations by returning a view that conforms to MapAnnotationProtocol, such as MapMarker, from the trailing closure of init(coordinateRegion:interactionModes:showsUserLocation:userTrackingMode:annotationItems:annotationContent:) or init(mapRect:interactionModes:showsUserLocation:userTrackingMode:annotationItems:annotationContent:). Items you provide as a collection to the source annotations need to conform to Identifiable.

For example, the following code displays a map with a marker annotation:

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

struct PinAnnotationMapView: View {
    let place: IdentifiablePlace
    @State var region: MKCoordinateRegion

    var body: some View {
        Map(coordinateRegion: $region,
            annotationItems: [place])
        { place in
            MapMarker(coordinate: place.location,
                   tint: Color.purple)
        }
    }
}

```

## Topics

### Creating a map marker

init(coordinate: CLLocationCoordinate2D, tint: Color?)

Creates a marker annotation at the map location you specify.

## Relationships

### Conforms To

- MapAnnotationProtocol

## See Also

### Structures

struct MapAnnotation

A customizable annotation that marks a map location.

Deprecated

struct MapPin

A pin-shaped annotation used to indicate a location on a map.

Deprecated

