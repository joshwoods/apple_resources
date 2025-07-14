

- MapKit
- MKMapView
-  overlays 

Instance Property

# overlays

The overlay objects associated with the map view.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var overlays: [any MKOverlay] { get }
```

## Discussion

This property contains the union of all overlays at the different levels of the map. The objects in this array adopt the MKOverlay protocol. If the map view has no associated no overlays, the value of this property is an empty array.

The order of the objects in this array doesn’t necessarily reflect their visual order on the map.

## See Also

### Accessing overlays

func overlays(in: MKOverlayLevel) -> [any MKOverlay]

Returns overlay objects in the specified level of the map.

func renderer(for: any MKOverlay) -> MKOverlayRenderer?

Returns the renderer object for drawing the contents of the specified overlay object.

enum MKOverlayLevel

Constants that indicate the position of overlays relative to other content.

func view(for: any MKOverlay) -> MKOverlayView

Returns the view associated with the overlay object, if any.

Deprecated

