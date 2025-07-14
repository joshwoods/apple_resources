

- MapKit
- MKMapView
-  addOverlay(\_:level:) 

Instance Method

# addOverlay(\_:level:)

Adds the overlay object to the map at the specified level.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func addOverlay(
    _ overlay: any MKOverlay,
    level: MKOverlayLevel
)
```

## Parameters 

`overlay`  

The overlay object to add. This object needs to conform to the MKOverlay protocol.

`level`  

The map level at which to place the overlay. For a list of possible values for this parameter, see MKOverlayLevel.

## Discussion

Positioning an overlay at a specific level places that overlay’s visual representation in front of or behind other map content such as map labels and point-of-interest icons.

This method adds the specified overlay to the end of the list of overlay objects at the given level. Adding an overlay also causes the map view to begin monitoring the area they represent. As soon as the bounding rectangle of the overlay intersects the visible portion of the map, the map view calls your delegate’s mapView(_:rendererFor:) method to get the renderer object to use when drawing the overlay.

To remove an overlay from a map, use the removeOverlay(_:) method.

## See Also

### Adding and inserting overlays

func addOverlays([any MKOverlay], level: MKOverlayLevel)

Adds an array of overlay objects to the map at the specified level.

func addOverlay(any MKOverlay)

Adds a single overlay object to the map.

func addOverlays([any MKOverlay])

Adds an array of overlay objects to the map.

func insertOverlay(any MKOverlay, at: Int, level: MKOverlayLevel)

Inserts an overlay object into the level at the specified index.

func insertOverlay(any MKOverlay, at: Int)

Inserts an overlay object into the list associated with the map.

func insertOverlay(any MKOverlay, above: any MKOverlay)

Inserts one overlay object above another.

func insertOverlay(any MKOverlay, below: any MKOverlay)

Inserts one overlay object below another.

func exchangeOverlay(any MKOverlay, with: any MKOverlay)

Exchanges the positions of two overlay objects.

func exchangeOverlay(at: Int, withOverlayAt: Int)

Exchanges the position of two overlay objects at the specified index.

