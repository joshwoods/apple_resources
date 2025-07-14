

- MapKit JS
- mapkit.PolygonOverlay
-  mapkit.PolygonOverlay 

Initializer

# mapkit.PolygonOverlay

Creates a polygon overlay with an array of points and style options.

MapKit JS 5.0+

``` source
new mapkit.PolygonOverlay(
 mapkit.Coordinate[] points,
 optional StylesOverlayOptions options
);
```

## Parameters 

`points`  

The points in the polygon as an array of arrays of mapkit.Coordinate, or an array of mapkit.Coordinate. For the latter, MapKit JS autowraps the array with an enclosing array.

`options`  

An optional object literal of options for initializing the polygon.

## Discussion

The following example shows the `options` parameter for a polygon overlay:

```
{
    style: new mapkit.Style({
        lineWidth: 2,
        strokeColor: "#F00",
        fillColor: "#339"
    }),
    selected: true
}
```

## See Also

### Creating a polygon overlay

StylesOverlayOptions

An observable set of style attributes for an overlay.

