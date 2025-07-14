

- MapKit JS
- mapkit.Style
-  lineGradient 

Instance Property

# lineGradient

The gradient to apply along the line.

MapKit JS 5.45+

``` source
attribute mapkit.LineGradient lineGradient;
```

## Discussion

If a style has both strokeColor and lineGradient definitions, MapKit JS displays the lineGradient. If you don’t define a color at the start or end location within the gradient, MapKit JS uses the style’s strokeColor as the default.

## See Also

### Styling lines

lineCap

The style to use when drawing line endings.

lineDash

An array of line and gap lengths for creating a dashed line.

lineDashOffset

The number of CSS pixels to use as an offset when drawing a line’s dash pattern.

lineJoin

The corner style to apply when joining line segments.

lineWidth

The width of a line’s stroke, in CSS pixels.

mapkit.LineGradient

A line that displays with a gradient along the length of the line.

