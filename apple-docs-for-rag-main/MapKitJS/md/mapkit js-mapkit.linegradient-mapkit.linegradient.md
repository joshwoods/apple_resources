

- MapKit JS
- mapkit.LineGradient
-  mapkit.LineGradient 

Initializer

# mapkit.LineGradient

Creates a style that renders a gradient along the length of a line.

MapKit JS 5.45+

``` source
new mapkit.LineGradient(
 optional Object options
);
```

## Parameters 

`options`  

A JavaScript object with unit distance values as keys with matched CSS colors.

## Mentioned in 

MapKit JS 5

## Discussion

The unit distance keys must be a number between `0` and `1`. A value of `0` represents the beginning of the polyline and a value of `1` represents the end. The associated values are CSS colors.

The following example creates a new gradient that progresses from `blue` at the start of the line to `red` at the end:

```
overlay.style.lineGradient = new mapkit.LineGradient({
    0: "blue",
    1: "red"
});
```

If the start or end of the line don’t have a defined color, the gradient uses the style’s strokeColor as a default.

You can extend gradients programatically with addColorStop and addColorStopAtIndex.

## See Also

### Creating a Line Gradient

addColorStop

Adds a color transition point to the gradient.

addColorStopAtIndex

Adds a color transition at the index point in the list of points within a polyline.

