

- MapKit JS
- mapkit.CircleOverlay
-  mapkit.CircleOverlay 

Initializer

# mapkit.CircleOverlay

Creates a circle overlay with a center coordinate, radius, and style options.

MapKit JS 5.0+

``` source
new mapkit.CircleOverlay(
 mapkit.Coordinate coordinate,
 number radius,
 optional StylesOverlayOptions options
);
```

## Parameters 

`coordinate`  

The required coordinate of the circle’s center.

`radius`  

The circle’s required radius, in meters.

`options`  

An optional object literal of overlay properties for initializing the circle.

## Discussion

An `options` parameter for a circle overlay resembles the following example:

```
{
    style: new mapkit.Style({
        lineWidth: 2,
        strokeColor: "#999",
        fillColor: "#FFF"
    }),
    data: {
        population: 30500
    },
    enabled: false
}
```

## See Also

### Creating a circle overlay

StylesOverlayOptions

An observable set of style attributes for an overlay.

