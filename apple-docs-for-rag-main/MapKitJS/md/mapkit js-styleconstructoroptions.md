

- MapKit JS
-  StyleConstructorOptions 

Structure

# StyleConstructorOptions

Initial values of options for applying style to overlays.

MapKit JS 5.0+

``` source
dictionary StyleConstructorOptions {
 string strokeColor;
 number strokeOpacity;
 number strokeStart;
 number strokeEnd;
 number lineWidth;
 string lineCap;
 string lineJoin;
 number[] lineDash;
 number lineDashOffset;
 mapkit.LineGradient lineGradient;
 string fillColor;
 number fillOpacity;
 string fillRule;
};
```

## Topics

### Setting fill styles

fillColor

The fill color of a shape.

fillOpacity

The opacity of the fill color.

fillRule

A rule for determining whether a point is inside or outside a polygon.

### Setting line styles

lineCap

The style to use when drawing line endings.

lineDash

An array of line and gap lengths for creating a dashed line.

lineDashOffset

The number of CSS pixels to use as the offset when drawing a line’s dash pattern.

lineJoin

The style to use when drawing joins between line segments.

lineWidth

The width of a line’s stroke, in CSS pixels.

### Setting stroke styles

strokeColor

The stroke color of a line.

strokeOpacity

The opacity of the stroke color.

strokeStart

The unit distance along the line where a stroke begins.

strokeEnd

The unit distance along the line where a stroke ends.

lineGradient

The gradient to apply along the line.

## See Also

### Creating a style

mapkit.Style

Creates and initializes a style object.

