

- GLKit
- GLKView
-  drawableWidth Deprecated

Instance Property

# drawableWidth

The width, in pixels, of the underlying framebuffer object.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
var drawableWidth: Int { get }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The height and width of the underlying framebuffer object is calculated automatically by the view object based on its bounds and contentScaleFactor properties and change whenever either of those properties change. Your application never directly adjusts the size of the framebuffer object. Instead, your application should read the drawableHeight and drawableWidth properties and use those to configure its OpenGL ES rendering code. For example, you might use the drawableHeight and drawableWidth properties to set the OpenGL ES viewport, determining the size and complexity of the art assets to load, and so on.

## See Also

### Read-only Framebuffer Properties

var drawableHeight: Int

The height, in pixels, of the underlying framebuffer object.

Deprecated

