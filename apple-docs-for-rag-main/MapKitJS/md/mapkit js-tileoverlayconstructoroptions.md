

- MapKit JS
-  TileOverlayConstructorOptions 

Structure

# TileOverlayConstructorOptions

Attributes for initializing a tile overlay, including minimum and maximum zoom, opacity, and custom data.

MapKit JS 5.0+

``` source
dictionary TileOverlayConstructorOptions {
 number minimumZ;
 number maximumZ;
 number opacity;
 Object data;
};
```

## Topics

### Initializing tile overlay options

data

Custom data for populating the URL template.

maximumZ

The maximum zoom level of the overlay.

minimumZ

The minimum zoom level of the overlay.

opacity

The opacity level of the overlay.

## See Also

### Creating a tile overlay

mapkit.TileOverlay

Creates a tile overlay with a URL template and style options.

