

- SceneKit
- SCNView
-  pixelFormat Deprecated

Instance Property

# pixelFormat

The view’s OpenGL pixel format.

macOS 10.8–10.14Deprecated

``` source
@MainActor
var pixelFormat: NSOpenGLPixelFormat? { get set }
```

Deprecated

OpenGL API deprecated, please use Metal instead. (Define SCN_SILENCE_GL_DEPRECATION to silence these warnings)

## Discussion

A pixel format object configures OpenGL attributes for rendering. For example, if you use OpenGL for custom rendering (see the SCNShadable, SCNNodeRendererDelegate, and SCNSceneRendererDelegate protocols), setting the pixel format to one that specifies the OpenGL 3.2 Core Profile allows you to use modern OpenGL APIs in your custom rendering code.

To change the pixel format, you can do either of the following:

- Set this property’s value before providing a scene for the view to render.

- In an SCNView subclass, override this property’s getter method to return your preferred pixel format.

## See Also

### Working with a View’s OpenGL Context

var openGLContext: NSOpenGLContext?

The OpenGL context that the view uses to render its contents.

Deprecated

