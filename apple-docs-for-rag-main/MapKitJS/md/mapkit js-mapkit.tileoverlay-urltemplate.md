

- MapKit JS
- mapkit.TileOverlay
-  urlTemplate 

Instance Property

# urlTemplate

A string, or callback function that returns a string, with a URL that provides the requested tile.

MapKit JS 5.0+

``` source
attribute string|Function urlTemplate;
```

## Discussion

MapKit JS sets the `urlTemplate` in the tile overlay constructor, and accesses or overrides it on the mapkit.TileOverlay object directly.

## See Also

### Customizing the tile overlay

data

A dictionary of custom properties to use with the URL template.

reload

Reloads the tile overlay for the displayed map region with the latest data values.

