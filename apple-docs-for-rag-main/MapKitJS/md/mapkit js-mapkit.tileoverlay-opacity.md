

- MapKit JS
- mapkit.TileOverlay
-  opacity 

Instance Property

# opacity

A number that indicates a tile’s opacity.

MapKit JS 5.0+

``` source
attribute number opacity;
```

## Discussion

Opacity can be a decimal value ranging from `0` to `1`, inclusive:

- An opacity value of `0` indicates tiles aren’t visible.

- An opacity value of `1` indicates tiles are completely opaque. A tile overlay with an opacity of `1` can still have an alpha channel and allow underlying overlays or the default tiles to show through.

The default value is `1`.

## See Also

### Setting overlay appearance

maximumZ

The maximum zoom level for a tile overlay.

minimumZ

The minimum zoom level for a tile overlay.

