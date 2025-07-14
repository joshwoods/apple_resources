

- MapKit
- MKMapView
-  addOverlay(\_:) 

Instance Method

# addOverlay(\_:)

Adds a single overlay object to the map.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func addOverlay(_ overlay: any MKOverlay)
```

## Parameters 

`overlay`  

The overlay object to add. This object needs to conform to the MKOverlay protocol.

## Discussion

The map view adds the specified object to the group of overlay objects in the MKOverlayLevel.aboveLabels level. Adding an overlay causes the map view to begin monitoring the area that the overlay represents. As soon as the bounding rectangle of an overlay intersects the visible portion of the map, the map view adds a corresponding overlay view to the map. Implement the mapView(_:rendererFor:) method of the map view’s delegate object to provide the overlay view.

To remove an overlay from a map, use the removeOverlay(_:) method.

## See Also

### Related Documentation

func removeOverlay(any MKOverlay)

Removes a single overlay object from the map.

func removeOverlays([any MKOverlay])

Removes one or more overlay objects from the map.

### Adding and inserting overlays

func addOverlay(any MKOverlay, level: MKOverlayLevel)

Adds the overlay object to the map at the specified level.

func addOverlays([any MKOverlay], level: MKOverlayLevel)

Adds an array of overlay objects to the map at the specified level.

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

