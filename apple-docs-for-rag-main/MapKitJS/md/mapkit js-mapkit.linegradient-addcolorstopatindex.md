

- MapKit JS
- mapkit.LineGradient
-  addColorStopAtIndex 

Instance Method

# addColorStopAtIndex

Adds a color transition at the index point in the list of points within a polyline.

MapKit JS 5.45+

``` source
void addColorStopAtIndex(
 number index,
 string color
);
```

## Parameters 

`index`  

A valid index into a polyline’s points.

`color`  

The CSS color at the index point.

## Discussion

If the index is invalid, MapKit JS logs a warning to the console, but doesn’t change the object.

## See Also

### Creating a Line Gradient

mapkit.LineGradient

Creates a style that renders a gradient along the length of a line.

addColorStop

Adds a color transition point to the gradient.

