

- AppKit
- NSGraphicsContext
-  shouldAntialias 

Instance Property

# shouldAntialias

A Boolean value that indicates whether the graphics context uses antialiasing.

macOS

``` source
var shouldAntialias: Bool { get set }
```

## Discussion

true if the receiver uses antialiasing. This value is part of the graphics state and is restored by restoreGraphicsState().

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

var patternPhase: NSPoint

The amount to offset the pattern color when filling the graphics context.

