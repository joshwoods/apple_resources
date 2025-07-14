

- AppKit
- NSStringDrawingContext
-  actualScaleFactor 

Instance Property

# actualScaleFactor

The actual scale factor that the system applied to the font during drawing.

macOS 10.11+

``` source
var actualScaleFactor: CGFloat { get }
```

## Discussion

If you specified a custom value in the minimumScaleFactor property, when drawing is complete, this property contains the actual scale factor value that was used to draw the string.

## See Also

### Accessing the scale factors

var minimumScaleFactor: CGFloat

The scale factor that determines the smallest font size to use during drawing.

