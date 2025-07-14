

- MapKit
-  MKTileOverlay 

Class

# MKTileOverlay

An overlay that covers an area of the map with tiles of bitmap images.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKTileOverlay
```

## Overview

You use tile overlay objects to represent your own tile-based content and to coordinate the display of that content in a map view. Your tiles can supplement the underlying map content or replace it completely. A tile overlay object coordinates the loading and management of the tiles, and a corresponding MKTileOverlayRenderer object handles the actual drawing of the tiles on the map.

You can use a single tile overlay object to represent all of the tiles at one or more zoom levels of the map. The default tile overlay object uses a template string to build URLs so that it can locate the map tiles it needs. Each URL incorporates the x and y index of the map tile, the zoom level it’s intended for, and the scale factor corresponding to the screen resolution on which to display the tile. The default class lets you specify map tiles with indexes that start in either the upper-left corner or lower-left corner of the map. If you use a different indexing scheme for your tiles, you can also subclass and override the url(forTilePath:) or loadTile(at:result:) methods to map between the requested tile and your custom indexing scheme.

## Topics

### Creating a tile overlay

init(urlTemplate: String?)

Creates and returns a tile overlay object using the specified tile-access template.

### Accessing the tile attributes

var tileSize: CGSize

The size (in pixels) of your tile images.

var isGeometryFlipped: Bool

A Boolean value that indicates the orientation of tile indexes along the y-axis.

var minimumZ: Int

The minimum zoom level that the tiles of this overlay object support.

var maximumZ: Int

The maximum zoom level that the tiles of this overlay object support.

var canReplaceMapContent: Bool

A Boolean value that indicates whether the tile content is fully opaque.

### Customizing the loading of tiles

var urlTemplate: String?

The template for generating tile image URLs.

func url(forTilePath: MKTileOverlayPath) -> URL

Returns the URL to use to access the specified tile.

func loadTile(at: MKTileOverlayPath, result: (Data?, (any Error)?) -> Void)

Loads the specified tile asynchronously.

struct MKTileOverlayPath

Values that specify the path indexes for a single overlay tile.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKAnnotation
- MKOverlay
- NSObjectProtocol

## See Also

### Tiled image overlays

class MKTileOverlayRenderer

The renderer for a tile overlay that handles the drawing of bitmap images on the map surface.

