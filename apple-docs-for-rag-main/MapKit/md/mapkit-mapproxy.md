

- MapKit
-  MapProxy 

Structure

# MapProxy

A proxy for accessing sizing information about a given map view.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct MapProxy
```

## Topics

### Creating a camera proxy

func camera(framing: MKCoordinateRegion) -> MapCamera

Creates a camera in the context of the map that frames the given coordinate region.

func camera(framing: MKMapRect) -> MapCamera

Creates a camera in the context of the map that frames the given map rectangle.

func camera(framing: MKMapItem, allowPitch: Bool) -> MapCamera

Creates a camera in the context of the map that frames the given map item.

### Converting between coordinate spaces

func convert(CLLocationCoordinate2D, to: some CoordinateSpaceProtocol) -> CGPoint?

Converts a map coordinate to a point in the specified coordinate space.

func convert(CGPoint, from: some CoordinateSpaceProtocol) -> CLLocationCoordinate2D?

Converts a point in the specified coordinate space to a map coordinate.

## See Also

### Structures

struct DefaultUserAnnotationContent

A structure that represents the view to show at the user’s location on the map.

struct EmptyMapContent

A map content element that doesn’t contain any content.

struct MapReader

A container view that defines its contents as a function of information about the first contained map.

struct TupleMapContent

A view created from a Swift tuple of map content values.

struct MapSelectableContentView

