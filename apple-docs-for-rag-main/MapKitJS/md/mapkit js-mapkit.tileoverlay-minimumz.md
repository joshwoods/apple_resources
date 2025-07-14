

- MapKit JS
- mapkit.TileOverlay
-  minimumZ 

Instance Property

# minimumZ

The minimum zoom level for a tile overlay.

MapKit JS 5.0+

``` source
attribute number minimumZ;
```

## Discussion

By default, the minimum zoom level for a tile overlay is the same as the minimum zoom level for MapKit JS built-in tiles. MapKit JS requests the overlay tiles when the map is above or at this zoom level.

The default value is `null`.

## See Also

### Setting overlay appearance

opacity

A number that indicates a tile’s opacity.

maximumZ

The maximum zoom level for a tile overlay.

