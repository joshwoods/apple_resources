

- MapKit
- MKMapView
-  overlays(in:) 

Instance Method

# overlays(in:)

Returns overlay objects in the specified level of the map.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func overlays(in level: MKOverlayLevel) -> [any MKOverlay]
```

## Parameters 

`level`  

The map level whose overlays you want. For a list of possible values for this parameter, see MKOverlayLevel.

## Return Value

An array of objects conforming to the MKOverlay protocol that display in the specified map level. If there are no overlays at the specified level, this method returns an empty array.

## Discussion

You can use this method to get all of the overlays assigned to a specific map level, which might be a subset of the complete set of overlay objects. For overlapping overlay objects, the order of objects in the array represents their visual order when displayed on the map, with objects in the beginning of the array located behind those at later indexes.

## See Also

### Related Documentation

func addOverlays([any MKOverlay], level: MKOverlayLevel)

Adds an array of overlay objects to the map at the specified level.

func addOverlay(any MKOverlay, level: MKOverlayLevel)

Adds the overlay object to the map at the specified level.

### Accessing overlays

var overlays: [any MKOverlay]

The overlay objects associated with the map view.

func renderer(for: any MKOverlay) -> MKOverlayRenderer?

Returns the renderer object for drawing the contents of the specified overlay object.

enum MKOverlayLevel

Constants that indicate the position of overlays relative to other content.

func view(for: any MKOverlay) -> MKOverlayView

Returns the view associated with the overlay object, if any.

Deprecated

