

- MapKit JS
- mapkit.TileOverlay
-  data 

Instance Property

# data

A dictionary of custom properties to use with the URL template.

MapKit JS 5.0+

``` source
attribute Object data;
```

## Discussion

The `data` object holds a dictionary of custom properties to fill the urlTemplate.

- If the urlTemplate is a callback, MapKit JS passes the entire data object as a parameter.

- If the urlTemplate is a string, `data` key names should match up with the custom placeholder names. MapKit JS ignores the keys that don’t exist in the URL template string.

The default value is `{}`.

This example shows adding a customized tile overlay to a map.

```
var customOverlay = new mapkit.TileOverlay("https://{subdomain}.customtileserver.com/{z}/{x}/{y}?scale={scale}&lang={lang}&imageFormat=jpg");
customOverlay.data = {
    subdomain: "staging",
    lang: mapkit.language
};
map.addTileOverlay(customOverlay);
```

------------------------------------------------------------------------

## See Also

### Customizing the tile overlay

urlTemplate

A string, or callback function that returns a string, with a URL that provides the requested tile.

reload

Reloads the tile overlay for the displayed map region with the latest data values.

