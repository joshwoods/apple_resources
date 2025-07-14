

- MapKit
- MKMapView
-  addOverlays(\_:) 

Instance Method

# addOverlays(\_:)

Adds an array of overlay objects to the map.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func addOverlays(_ overlays: [any MKOverlay])
```

## Parameters 

`overlays`  

An array of objects, each of which needs to conform to the MKOverlay protocol.

## Discussion

The map view adds the specified objects to the group of overlay objects in the MKOverlayLevel.aboveLabels level. Adding an overlay causes the map view to begin monitoring the area that the overlay represents. As soon as the bounding rectangle of the overlay intersects the visible portion of the map, the map view tries to draw the overlay, or adds the corresponding overlay view to the map. Implement the mapView(_:rendererFor:) method of the map view’s delegate object to provide the overlay view.

To remove multiple overlays from a map, use the removeOverlays(_:) method.

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

func addOverlay(any MKOverlay)

Adds a single overlay object to the map.

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

