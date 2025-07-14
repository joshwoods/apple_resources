

- AppKit
- NSGraphicsContext
-  imageInterpolation 

Instance Property

# imageInterpolation

A constant that specifies the graphics context’s interpolation, or image smoothing, behavior.

macOS

``` source
var imageInterpolation: NSImageInterpolation { get set }
```

## Discussion

Note that this value is not part of the graphics state, so it cannot be reset using restoreGraphicsState().

## See Also

### Configuring Rendering Options

var compositingOperation: NSCompositingOperation

The graphics context’s global compositing operation setting.

enum NSCompositingOperation

Constants that describe compositing operators in terms of source and destination images, each having an opaque and transparent region.

enum NSImageInterpolation

Constants that specify the interpolation, or image smoothing, behavior used by the image interpolation property.

var shouldAntialias: Bool

A Boolean value that indicates whether the graphics context uses antialiasing.

var patternPhase: NSPoint

The amount to offset the pattern color when filling the graphics context.

