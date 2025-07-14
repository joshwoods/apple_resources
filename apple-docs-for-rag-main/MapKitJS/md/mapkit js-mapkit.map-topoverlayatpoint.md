

- MapKit JS
- mapkit.Map
-  topOverlayAtPoint 

Instance Method

# topOverlayAtPoint

Returns the topmost overlay at a given point on the webpage.

MapKit JS 5.0+

``` source
mapkit.Overlay topOverlayAtPoint(
 DOMPoint point
);
```

## Parameters 

`point`  

A point in the page’s coordinate system, such as `new DOMPoint(event.pageX, event.pageY)` when handling a mouse event.

## Return Value

Returns the topmost overlay or `null`.

## Discussion

If there are multiple overlays at a point, MapKit JS returns the overlay closest to the foreground. If the user selects an overlay, MapKit JS draws user-selected overlays on top of all other overlays. So when a user selects an overlay, MapKit JS returns that overlay.

The following code example identifies the topmost overlay during a mouse move event:

```
document.querySelector(".mk-map-view").addEventListener("mousemove", function(event) {
    var targetOverlay = map.topOverlayAtPoint(new DOMPoint(event.pageX, event.pageY));
    // Add special styling to the overlay to indicate its hover state or whatever you want.
    // ...
});

```

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

addOverlays

Adds multiple overlays to the map.

removeOverlay

Removes an overlay from the map.

removeOverlays

Removes multiple overlays from the map.

