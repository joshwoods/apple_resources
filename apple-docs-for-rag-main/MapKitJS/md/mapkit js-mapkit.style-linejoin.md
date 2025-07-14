

- MapKit JS
- mapkit.Style
-  lineJoin 

Instance Property

# lineJoin

The corner style to apply when joining line segments.

MapKit JS 5.0+

``` source
attribute string lineJoin;
```

## Discussion

The three options for line joins are `miter` (join is a sharp corner), `round` (join is a rounded corner), or `bevel` (join is a beveled corner). The default line join is `round`.

## See Also

### Styling lines

lineCap

The style to use when drawing line endings.

lineDash

An array of line and gap lengths for creating a dashed line.

lineDashOffset

The number of CSS pixels to use as an offset when drawing a line’s dash pattern.

lineWidth

The width of a line’s stroke, in CSS pixels.

lineGradient

The gradient to apply along the line.

mapkit.LineGradient

A line that displays with a gradient along the length of the line.

