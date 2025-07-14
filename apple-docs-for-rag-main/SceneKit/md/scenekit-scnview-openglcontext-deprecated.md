

- SceneKit
- SCNView
-  openGLContext Deprecated

Instance Property

# openGLContext

The OpenGL context that the view uses to render its contents.

macOS 10.8–10.14Deprecated

``` source
@MainActor
var openGLContext: NSOpenGLContext? { get set }
```

Deprecated

OpenGL API deprecated, please use Metal instead. (Define SCN_SILENCE_GL_DEPRECATION to silence these warnings)

## Discussion

If you use OpenGL for custom rendering (see the SCNShadable, SCNNodeRendererDelegate, and SCNSceneRendererDelegate protocols), you can use this property to share OpenGL resources between the context used for rendering the scene and other OpenGL contexts your app uses. For details on sharing OpenGL resources, see Sharing Rendering Context Resources. (SceneKit automatically shares its own OpenGL resources between multiple SCNView instances in your app as needed.)

## See Also

### Working with a View’s OpenGL Context

var pixelFormat: NSOpenGLPixelFormat?

The view’s OpenGL pixel format.

Deprecated

