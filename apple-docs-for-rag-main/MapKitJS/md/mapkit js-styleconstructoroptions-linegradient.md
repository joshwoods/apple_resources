

- MapKit JS
- StyleConstructorOptions
-  lineGradient 

Instance Property

# lineGradient

The gradient to apply along the line.

MapKit JS 5.45+

``` source
attribute mapkit.LineGradient lineGradient;
```

## Discussion

If a style has both strokeColor and lineGradient definitions, lineGradient takes precedence and displays. If you don’t define a color at the start or end location within the gradient, MapKit JS uses the style’s strokeColor.

## See Also

### Setting stroke styles

strokeColor

The stroke color of a line.

strokeOpacity

The opacity of the stroke color.

strokeStart

The unit distance along the line where a stroke begins.

strokeEnd

The unit distance along the line where a stroke ends.

