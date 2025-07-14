

- MapKit
- MKMapView
-  exchangeOverlay(\_:with:) 

Instance Method

# exchangeOverlay(\_:with:)

Exchanges the positions of two overlay objects.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func exchangeOverlay(
    _ overlay1: any MKOverlay,
    with overlay2: any MKOverlay
)
```

## Parameters 

`overlay1`  

The first overlay object.

`overlay2`  

The second overlay object.

## Discussion

If the overlays are in the same map level, they exchange positions within that level’s array of overlay objects. If they’re in different map levels, the two objects also swap levels. Swapping the position of the overlays affects their visibility in the map view.

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

func insertOverlay(any MKOverlay, above: any MKOverlay)

Inserts one overlay object above another.

func insertOverlay(any MKOverlay, below: any MKOverlay)

Inserts one overlay object below another.

func exchangeOverlay(at: Int, withOverlayAt: Int)

Exchanges the position of two overlay objects at the specified index.

