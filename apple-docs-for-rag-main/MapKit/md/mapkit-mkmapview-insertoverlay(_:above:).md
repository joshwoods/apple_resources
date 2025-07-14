

- MapKit
- MKMapView
-  insertOverlay(\_:above:) 

Instance Method

# insertOverlay(\_:above:)

Inserts one overlay object above another.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func insertOverlay(
    _ overlay: any MKOverlay,
    above sibling: any MKOverlay
)
```

## Parameters 

`overlay`  

The overlay object to insert.

`sibling`  

An existing object in the overlays array. This object needs to exist in the array and can’t be `nil`.

## Discussion

This method inserts the overlay into the MKOverlayLevel.aboveLabels level and positions it relative to the specified sibling. When displaying it, the map view displays the overlay’s contents above that of its sibling. If the sibling isn’t in the same map level, this method appends the overlay to the end of the list of overlays at the indicated level.

## See Also

### Adding and inserting overlays

func addOverlay(any MKOverlay, level: MKOverlayLevel)

Adds the overlay object to the map at the specified level.

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

func insertOverlay(any MKOverlay, below: any MKOverlay)

Inserts one overlay object below another.

func exchangeOverlay(any MKOverlay, with: any MKOverlay)

Exchanges the positions of two overlay objects.

func exchangeOverlay(at: Int, withOverlayAt: Int)

Exchanges the position of two overlay objects at the specified index.

