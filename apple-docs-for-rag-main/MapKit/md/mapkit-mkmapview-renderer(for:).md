

- MapKit
- MKMapView
-  renderer(for:) 

Instance Method

# renderer(for:)

Returns the renderer object for drawing the contents of the specified overlay object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func renderer(for overlay: any MKOverlay) -> MKOverlayRenderer?
```

## Parameters 

`overlay`  

The overlay object whose renderer you want.

## Return Value

The renderer object in use for the specified overlay or `nil` if the overlay is not onscreen.

## Discussion

This method returns the renderer object that your map delegate provided in its mapView(_:rendererFor:) method.

## See Also

### Accessing overlays

var overlays: [any MKOverlay]

The overlay objects associated with the map view.

func overlays(in: MKOverlayLevel) -> [any MKOverlay]

Returns overlay objects in the specified level of the map.

enum MKOverlayLevel

Constants that indicate the position of overlays relative to other content.

func view(for: any MKOverlay) -> MKOverlayView

Returns the view associated with the overlay object, if any.

Deprecated

