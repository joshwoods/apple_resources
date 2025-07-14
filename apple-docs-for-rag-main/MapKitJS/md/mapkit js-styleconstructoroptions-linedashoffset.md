

- MapKit JS
- StyleConstructorOptions
-  lineDashOffset 

Instance Property

# lineDashOffset

The number of CSS pixels to use as the offset when drawing a line’s dash pattern.

MapKit JS 5.0+

``` source
attribute number lineDashOffset;
```

## Discussion

This has no effect if you set `lineDash` to draw solid lines by setting this property to an empty array. The default line dash offset is `0`.

## See Also

### Setting line styles

lineCap

The style to use when drawing line endings.

lineDash

An array of line and gap lengths for creating a dashed line.

lineJoin

The style to use when drawing joins between line segments.

lineWidth

The width of a line’s stroke, in CSS pixels.

