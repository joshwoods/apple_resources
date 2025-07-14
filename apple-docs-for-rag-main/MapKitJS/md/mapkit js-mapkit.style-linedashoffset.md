

- MapKit JS
- mapkit.Style
-  lineDashOffset 

Instance Property

# lineDashOffset

The number of CSS pixels to use as an offset when drawing a line’s dash pattern.

MapKit JS 5.0+

``` source
attribute number lineDashOffset;
```

## Discussion

This has no effect if you set `lineDash` to draw solid lines. The default line dash offset is `0`.

## See Also

### Styling lines

lineCap

The style to use when drawing line endings.

lineDash

An array of line and gap lengths for creating a dashed line.

lineJoin

The corner style to apply when joining line segments.

lineWidth

The width of a line’s stroke, in CSS pixels.

lineGradient

The gradient to apply along the line.

mapkit.LineGradient

A line that displays with a gradient along the length of the line.

