

- MapKit
- MKMapView
-  insertOverlay(\_:at:level:) 

Instance Method

# insertOverlay(\_:at:level:)

Inserts an overlay object into the level at the specified index.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func insertOverlay(
    _ overlay: any MKOverlay,
    at index: Int,
    level: MKOverlayLevel
)
```

## Parameters 

`overlay`  

The overlay object to insert.

`index`  

The index at which to insert the overlay object. If this value is greater than the number of objects in the overlays property, this method appends the object to the end of the array.

`level`  

The map level at which to place the overlay. For a list of possible values for this parameter, see MKOverlayLevel.

## Discussion

Inserting an overlay at a specific level places that overlay’s visual representation in front of or behind other map content such as map labels and point-of-interest icons.

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

