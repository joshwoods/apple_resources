

- MapKit JS
- mapkit.Map
-  overlays 

Instance Property

# overlays

An array of all of the map’s overlays.

MapKit JS 5.0+

``` source
attribute mapkit.Overlay[] overlays;
```

## Discussion

You can set this attribute to a new (possibly empty) array of overlays to update or delete all the overlays on the map.

## See Also

### Adding and removing overlays

selectedOverlay

The selected overlay on the map.

overlaysAtPoint

Returns an array of overlays at a given point on the webpage.

addOverlay

Adds an overlay to the map.

addOverlays

Adds multiple overlays to the map.

removeOverlay

Removes an overlay from the map.

removeOverlays

Removes multiple overlays from the map.

topOverlayAtPoint

Returns the topmost overlay at a given point on the webpage.

