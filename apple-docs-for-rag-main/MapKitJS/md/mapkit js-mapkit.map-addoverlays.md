

- MapKit JS
- mapkit.Map
-  addOverlays 

Instance Method

# addOverlays

Adds multiple overlays to the map.

MapKit JS 5.0+

``` source
mapkit.Overlay[] addOverlays(
 mapkit.Overlay[] overlays
);
```

## Parameters 

`overlays`  

An array of overlays to add.

## Return Value

Returns the array of overlays.

## Discussion

MapKit JS adds the overlays to the end of the map’s overlays array.

## See Also

### Adding and removing overlays

overlays

An array of all of the map’s overlays.

selectedOverlay

The selected overlay on the map.

overlaysAtPoint

Returns an array of overlays at a given point on the webpage.

addOverlay

Adds an overlay to the map.

removeOverlay

Removes an overlay from the map.

removeOverlays

Removes multiple overlays from the map.

topOverlayAtPoint

Returns the topmost overlay at a given point on the webpage.

