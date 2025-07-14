

- MapKit JS
- StyleConstructorOptions
-  lineJoin 

Instance Property

# lineJoin

The style to use when drawing joins between line segments.

MapKit JS 5.0+

``` source
attribute string lineJoin;
```

## Discussion

The three options for line joins are `miter` (the join is a sharp corner), `round` (the join is a rounded corner), or `bevel` (the join is a beveled corner). The default line join is `round`.

## See Also

### Setting line styles

lineCap

The style to use when drawing line endings.

lineDash

An array of line and gap lengths for creating a dashed line.

lineDashOffset

The number of CSS pixels to use as the offset when drawing a line’s dash pattern.

lineWidth

The width of a line’s stroke, in CSS pixels.

