

- AppKit
- NSOpenGLView
-  wantsExtendedDynamicRangeOpenGLSurface Deprecated

Instance Property

# wantsExtendedDynamicRangeOpenGLSurface

Enables extended dynamic range values on the screen.

macOS 10.11–10.14Deprecated

``` source
@MainActor
var wantsExtendedDynamicRangeOpenGLSurface: Bool { get set }
```

Deprecated

OpenGL API deprecated; please use Metal and MetalKit. (Define GL_SILENCE_DEPRECATION to silence these warnings.)

## Discussion

If any view on the screen has this enabled, the screen which the OpenGL surface is on may have its `maximumExtendedDynamicRangeColorComponentValue` value increased. When composited by the Window Server, color values rendered by this OpenGL surface will be clamped to the screen’s `maximumExtendedDynamicRangeColorComponentValue` value rather than `1.0`.

## See Also

### Related Documentation

var maximumExtendedDynamicRangeColorComponentValue: CGFloat

The current maximum color component value for the screen.

