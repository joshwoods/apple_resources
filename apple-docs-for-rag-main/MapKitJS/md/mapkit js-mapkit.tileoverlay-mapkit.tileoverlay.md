

- MapKit JS
- mapkit.TileOverlay
-  mapkit.TileOverlay 

Initializer

# mapkit.TileOverlay

Creates a tile overlay with a URL template and style options.

MapKit JS 5.0+

``` source
new mapkit.TileOverlay(
 string|function urlTemplate,
 optional TileOverlayConstructorOptions options
);
```

## Parameters 

`urlTemplate`  

The urlTemplate can be in the format of a template URL string or a function that returns a URL string from a set of tile parameters. MapKit JS requests new tiles when the map zooms or pans, the display changes, or the custom data properties change.

- The template string must be in the format: `https://myserver/tile?x={x}&y={y}&z={z}&scale={scale}`. MapKit JS replaces the `x`, `y`, `z`, and `scale` values depending on the displayed map region and screen resolution, then loads an image from that URL. You can also add custom values to the template string. For example, a template string could look like: `https://{subdomain}.customtileserver.com/{z}/{x}/{y}?lang={lang}`. In this case, you must define `TileOverlay.data.subdomain` and `TileOverlay.data.lang` for the placeholders to populate. Also, note that not all parameters are necessary in a template string. The `scale` parameter is absent in this example.

- You can provide a callback function instead of the template string. When MapKit JS needs to request new tiles, it invokes the urlTemplate callback with the parameters `x`, `y`, `z`, `scale`, and `data`. The callback function must return a URL for the provided parameters. If the return value is anything but a nonempty string, MapKit JS doesn’t load any tiles for the requested region.

`options`  

An optional object literal of properties for initializing the tile overlay. These properties include minimumZ, maximumZ, opacity, and data.

## See Also

### Creating a tile overlay

TileOverlayConstructorOptions

Attributes for initializing a tile overlay, including minimum and maximum zoom, opacity, and custom data.

