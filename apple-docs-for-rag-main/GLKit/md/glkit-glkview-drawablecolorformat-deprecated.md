

- GLKit
- GLKView
-  drawableColorFormat Deprecated

Instance Property

# drawableColorFormat

The format of the color renderbuffer.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
var drawableColorFormat: GLKViewDrawableColorFormat { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The default value is GLKViewDrawableColorFormat.RGBA8888.

After your application changes the value of this property, the view recreates its framebuffer object the next time the view is drawn.

## See Also

### Configuring the Framebuffer Object

var drawableDepthFormat: GLKViewDrawableDepthFormat

The format of the depth renderbuffer

Deprecated

var drawableStencilFormat: GLKViewDrawableStencilFormat

The format of the stencil renderbuffer.

Deprecated

var drawableMultisample: GLKViewDrawableMultisample

The format of the multisampling buffer.

Deprecated

