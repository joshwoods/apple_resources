

- MapKit
-  MapPin Deprecated

Structure

# MapPin

A pin-shaped annotation used to indicate a location on a map.

MapKitSwiftUIiOS 14.0–16.0DeprecatediPadOS 14.0–16.0DeprecatedMac CatalystmacOS 11.0–13.0DeprecatedtvOS 14.0–16.0DeprecatedvisionOSwatchOS 7.0–9.0Deprecated

``` source
struct MapPin
```

Deprecated

Use Marker along with Map initializers that take a MapContentBuilder instead.

## Overview

Create a Map and display pin annotations by returning a view that conforms to MapAnnotationProtocol, such as MapPin, from the trailing closure of init(coordinateRegion:interactionModes:showsUserLocation:userTrackingMode:annotationItems:annotationContent:) or init(mapRect:interactionModes:showsUserLocation:userTrackingMode:annotationItems:annotationContent:). Items you provide as a collection to the source annotations need to conform to Identifiable.

For example, the following code displays a map with a pin annotation:

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
            MapPin(coordinate: place.location,
                   tint: Color.purple)
        }
    }
}
```

## Topics

### Creating a map pin

init(coordinate: CLLocationCoordinate2D, tint: Color?)

Creates a map pin at the map location that you specify.

## Relationships

### Conforms To

- MapAnnotationProtocol

## See Also

### Structures

struct MapAnnotation

A customizable annotation that marks a map location.

Deprecated

struct MapMarker

A balloon-shaped annotation used to indicate the location on a map.

Deprecated

