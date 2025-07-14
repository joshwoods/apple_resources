

- AppKit
-  NSOpenGLPFAAllowOfflineRenderers Deprecated

Global Variable

# NSOpenGLPFAAllowOfflineRenderers

A Boolean attribute. If present, this attribute indicates that offline renderers may be used.

macOS 10.5–10.14Deprecated

``` source
var NSOpenGLPFAAllowOfflineRenderers: Int { get }
```

Deprecated

OpenGL API deprecated; please use Metal and MetalKit. (Define GL_SILENCE_DEPRECATION to silence these warnings.)

## See Also

### Constants

var NSOpenGLPFAAccelerated: Int

A Boolean attribute. If present, this attribute indicates that only hardware-accelerated renderers are considered. If not present, accelerated renderers are still preferred.

Deprecated

var NSOpenGLPFAAcceleratedCompute: Int

If present, this attribute indicates that only renderers that can execute OpenCL programs should be used.

Deprecated

var NSOpenGLPFAAccumSize: Int

Value is a nonnegative buffer size specification. An accumulation buffer that most closely matches the specified size is preferred.

Deprecated

var NSOpenGLPFAAllRenderers: Int

A Boolean attribute. If present, this attribute indicates that the pixel format selection is open to all available renderers, including debug and special-purpose renderers that are not OpenGL compliant.

Deprecated

var NSOpenGLPFAAlphaSize: Int

Value is a nonnegative buffer size specification. An alpha buffer that most closely matches the specified size is preferred.

Deprecated

var NSOpenGLPFAAuxBuffers: Int

Value is a nonnegative integer that indicates the desired number of auxiliary buffers. Pixel formats with the smallest number of auxiliary buffers that meets or exceeds the specified number are preferred.

Deprecated

var NSOpenGLPFAAuxDepthStencil: Int

Each auxiliary buffer has its own depth stencil.

Deprecated

var NSOpenGLPFABackingStore: Int

A Boolean attribute. If present, this attribute indicates that OpenGL only considers renderers that have a back color buffer the full size of the drawable (regardless of window visibility) and that guarantee the back buffer contents to be valid after a call to `NSOpenGLContext` object’s flushBuffer().

Deprecated

var NSOpenGLPFAClosestPolicy: Int

A Boolean attribute. If present, this attribute indicates that the pixel format choosing policy is altered for the color buffer such that the buffer closest to the requested size is preferred, regardless of the actual color buffer depth of the supported graphics device.

Deprecated

var NSOpenGLPFAColorFloat: IntDeprecated

var NSOpenGLPFAColorSize: Int

Value is a nonnegative buffer size specification. A color buffer that most closely matches the specified size is preferred. If unspecified, OpenGL chooses a color size that matches the screen.

Deprecated

var NSOpenGLPFADepthSize: Int

Value is a nonnegative depth buffer size specification. A depth buffer that most closely matches the specified size is preferred.

Deprecated

var NSOpenGLPFADoubleBuffer: Int

A Boolean attribute. If present, this attribute indicates that only double-buffered pixel formats are considered. Otherwise, only single-buffered pixel formats are considered.

Deprecated

var NSOpenGLPFAMaximumPolicy: Int

A Boolean attribute. If present, this attribute indicates that the pixel format choosing policy is altered for the color, depth, and accumulation buffers such that, if a nonzero buffer size is requested, the largest available buffer is preferred.

Deprecated

var NSOpenGLPFAMinimumPolicy: Int

A Boolean attribute. If present, this attribute indicates that the pixel format choosing policy is altered for the color, depth, and accumulation buffers such that only buffers of size greater than or equal to the desired size are considered.

Deprecated

