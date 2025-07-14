

- MapKit
- MKMapView
-  view(for:) Deprecated

Instance Method

# view(for:)

Returns the view associated with the overlay object, if any.

iOS 4.0–13.0DeprecatediPadOS 4.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func view(for overlay: any MKOverlay) -> MKOverlayView
```

Deprecated

Use the renderer(for:) method instead.

## Parameters 

`overlay`  

The overlay object whose view you want.

## Return Value

The view associated with the overlay object or `nil` if the overlay is not onscreen.

## See Also

### Accessing overlays

var overlays: [any MKOverlay]

The overlay objects associated with the map view.

func overlays(in: MKOverlayLevel) -> [any MKOverlay]

Returns overlay objects in the specified level of the map.

func renderer(for: any MKOverlay) -> MKOverlayRenderer?

Returns the renderer object for drawing the contents of the specified overlay object.

enum MKOverlayLevel

Constants that indicate the position of overlays relative to other content.

