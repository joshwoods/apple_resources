

- MapKit
- MKTileOverlayRenderer
-  init(tileOverlay:) 

Initializer

# init(tileOverlay:)

Initializes and returns a tile renderer with the specified overlay object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
init(tileOverlay overlay: MKTileOverlay)
```

## Parameters 

`overlay`  

The tile overlay object whose contents you want to draw.

## Return Value

An initialized tile renderer object.

## Discussion

The returned renderer object works with the tile overlay object to coordinate the loading and display of its map tiles.

## See Also

### Related Documentation

Location and Maps Programming Guide

