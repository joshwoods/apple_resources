

- MapKit JS
- mapkit.Map
-  selectedOverlay 

Instance Property

# selectedOverlay

The selected overlay on the map.

MapKit JS 5.0+

``` source
attribute mapkit.Overlay selectedOverlay;
```

## Discussion

To deselect any selected overlay, set this attribute to `null`.

To select an overlay that’s already part of the map, set this attribute to the desired overlay.

When MapKit JS removes the selected overlay from the map (as an effect of removeOverlay, removeOverlays, or setting a new set of overlays with the overlays property), MapKit JS deselects the overlay before removing it.

## See Also

### Adding and removing overlays

overlays

An array of all of the map’s overlays.

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

