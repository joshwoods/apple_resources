

- MapKit
-  MKTileOverlayRenderer 

Class

# MKTileOverlayRenderer

The renderer for a tile overlay that handles the drawing of bitmap images on the map surface.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKTileOverlayRenderer
```

## Overview

You create instances of this class when tile overlays become visible on the map view. A renderer works closely with its associated tile overlay object to coordinate the loading and drawing of tiles at appropriate times.

For information about how to specify the tiles to display on the map, see MKTileOverlay.

## Topics

### Creating a tile renderer

init(tileOverlay: MKTileOverlay)

Initializes and returns a tile renderer with the specified overlay object.

### Reloading the tile data

func reloadData()

Forces the tile overlay renderer to reload and redisplay the tiles.

## Relationships

### Inherits From

- MKOverlayRenderer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Tiled image overlays

class MKTileOverlay

An overlay that covers an area of the map with tiles of bitmap images.

