

- MapKit
- Marker
-  init(\_:monogram:coordinate:) 

Initializer

# init(\_:monogram:coordinate:)

Creates a marker at the given location with the provided title string and monogram.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    _ title: S,
    monogram: Text,
    coordinate: CLLocationCoordinate2D
) where Label == Label, S : StringProtocol
```

## Parameters 

`title`  

The title of the marker.

`monogram`  

A Text view that contains up to three characters to display on the marker’s balloon.

`coordinate`  

The coordinate used to display the marker.

## See Also

### Creating a marker

init&lt;S>(S, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the label you provide.

init&lt;S>(S, image: String, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the provided title and image resource to display as the balloon’s icon.

init&lt;S>(S, systemImage: String, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the provided title and a system image the map displays as the balloon’s icon.

init(LocalizedStringKey, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the localized string key you provide.

init(LocalizedStringKey, image: String, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the provided localized title and image resource to display as the balloon’s icon.

init(LocalizedStringKey, monogram: Text, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with the provided title key and monogram.

init(LocalizedStringKey, systemImage: String, coordinate: CLLocationCoordinate2D)

Creates a marker at the given location with a localized title, and a system image the map displays as the balloon’s icon.

init(coordinate: CLLocationCoordinate2D, label: () -> Label)

Creates a marker at the given location with the provided label.

init(item: MKMapItem)

Creates a marker for a given map item using a MapKit-provided label.

