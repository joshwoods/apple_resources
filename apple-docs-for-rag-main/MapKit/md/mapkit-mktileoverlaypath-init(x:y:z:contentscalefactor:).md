

- MapKit
- MKTileOverlayPath
-  init(x:y:z:contentScaleFactor:) 

Initializer

# init(x:y:z:contentScaleFactor:)

Creates a new overlay path with the specified indexes and content scale factor.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    x: Int,
    y: Int,
    z: Int,
    contentScaleFactor: CGFloat
)
```

## Parameters 

`x`  

The index of the tile along the x-axis of the map.

`y`  

The index of the tile along the y-axis of the map.

`z`  

The index of the tile along the z-axis of the map.

`contentScaleFactor`  

The screen scale that the framework shows the tile. This value is typically either `1.0` (for standard resolution displays) or `2.0` (for Retina displays).

## See Also

### Creating a tile overlay path

init()

Creates a new tile overlay path.

