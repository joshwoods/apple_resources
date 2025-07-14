

- GLKit
- GLKView
-  drawableDepthFormat Deprecated

Instance Property

# drawableDepthFormat

The format of the depth renderbuffer

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
var drawableDepthFormat: GLKViewDrawableDepthFormat { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The default value is GLKViewDrawableDepthFormat.formatNone.

After your application changes the value of this property, the view recreates its framebuffer object the next time the view is drawn.

## See Also

### Configuring the Framebuffer Object

var drawableColorFormat: GLKViewDrawableColorFormat

The format of the color renderbuffer.

Deprecated

var drawableStencilFormat: GLKViewDrawableStencilFormat

The format of the stencil renderbuffer.

Deprecated

var drawableMultisample: GLKViewDrawableMultisample

The format of the multisampling buffer.

Deprecated

