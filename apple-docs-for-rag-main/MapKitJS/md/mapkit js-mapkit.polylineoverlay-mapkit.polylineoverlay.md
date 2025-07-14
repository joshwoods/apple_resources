

- MapKit JS
- mapkit.PolylineOverlay
-  mapkit.PolylineOverlay 

Initializer

# mapkit.PolylineOverlay

Creates a polyline overlay with coordinate points and style options.

MapKit JS 5.0+

``` source
new mapkit.PolylineOverlay(
 mapkit.Coordinate[] points,
 optional StylesOverlayOptions options
);
```

## Parameters 

`points`  

The required points in the polyline as an array of mapkit.Coordinate.

`options`  

An optional object literal of style options for initializing the polyline.

## Discussion

The following is an example of the `options` parameter for a polyline overlay:

```
{
    style: new mapkit.Style({
        lineWidth: 2,
        strokeColor: "#F0F"
    })
}
```

## See Also

### Creating a polyline overlay

StylesOverlayOptions

An observable set of style attributes for an overlay.

