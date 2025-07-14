

- AppKit
- NSGraphicsContext
-  patternPhase 

Instance Property

# patternPhase

The amount to offset the pattern color when filling the graphics context.

macOS

``` source
var patternPhase: NSPoint { get set }
```

## Discussion

Use this property when you need to line up the pattern color with another pattern, such as the pattern in a superview. The pattern phase is a translation (width, height) applied before a pattern is drawn in the current context and is part of the saved graphics state of the context. The default pattern phase is (0,0). Setting the pattern phase has the effect of temporarily changing the pattern matrix of any pattern you decide to draw. For example, setting the pattern phase to (2,3) has the effect of moving the start of pattern cell tiling to the point (2,3) in default user space.

## See Also

### Configuring Rendering Options

var compositingOperation: NSCompositingOperation

The graphics context’s global compositing operation setting.

enum NSCompositingOperation

Constants that describe compositing operators in terms of source and destination images, each having an opaque and transparent region.

var imageInterpolation: NSImageInterpolation

A constant that specifies the graphics context’s interpolation, or image smoothing, behavior.

enum NSImageInterpolation

Constants that specify the interpolation, or image smoothing, behavior used by the image interpolation property.

var shouldAntialias: Bool

A Boolean value that indicates whether the graphics context uses antialiasing.

