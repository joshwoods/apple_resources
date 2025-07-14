

- MapKit JS
- mapkit.TileOverlay
-  maximumZ 

Instance Property

# maximumZ

The maximum zoom level for a tile overlay.

MapKit JS 5.0+

``` source
attribute number maximumZ;
```

## Discussion

The `maximumZ` value defaults to the maximum zoom level of MapKit JS tiles. The zoom level can go higher and expands the map’s zoom range, if necessary. MapKit JS requests the overlay tiles when the map is below or at this zoom level.

The default value is `null`.

## See Also

### Setting overlay appearance

opacity

A number that indicates a tile’s opacity.

minimumZ

The minimum zoom level for a tile overlay.

