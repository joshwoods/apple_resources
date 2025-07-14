

- MapKit JS
- mapkit.LineGradient
-  addColorStop 

Instance Method

# addColorStop

Adds a color transition point to the gradient.

MapKit JS 5.45+

``` source
void addColorStop(
 number offset,
 string color
);
```

## Parameters 

`offset`  

The unit distance at which to add the color.

`color`  

The CSS color at the transition point.

## Discussion

If offset is less than `0` or greater than `1`, MapKit JS logs a warning to the console, but doesn’t change the object.

## See Also

### Creating a Line Gradient

mapkit.LineGradient

Creates a style that renders a gradient along the length of a line.

addColorStopAtIndex

Adds a color transition at the index point in the list of points within a polyline.

