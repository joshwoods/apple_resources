

- SceneKit
- SCNView
-  eaglContext Deprecated

Instance Property

# eaglContext

The OpenGL ES context that the view uses to render its contents.

iOS 8.0–12.0DeprecatediPadOS 8.0–12.0DeprecatedtvOSDeprecated

``` source
@MainActor
var eaglContext: EAGLContext? { get set }
```

Deprecated

OpenGL API deprecated, please use Metal instead. (Define SCN_SILENCE_GL_DEPRECATION to silence these warnings)

## Discussion

If you use OpenGL ES for custom rendering (see the SCNShadable, SCNNodeRendererDelegate, and SCNSceneRendererDelegate protocols), you can use this property to share OpenGL ES resources between the context used for rendering the scene and other OpenGL ES contexts your app uses. For details on sharing OpenGL ES resources, see An EAGL Sharegroup Manages OpenGL ES Objects for the Context. (SceneKit automatically shares its own OpenGL ES resources between multiple SCNView instances in your app as needed.)

If you supply your own EAGLContext object for a SceneKit view, specify the OpenGL ES 2.0 or 3.0 API when creating it. SceneKit supports OpenGL ES 3.0, but some features are disabled when rendering in an OpenGL ES 3.0 context. SceneKit does not support OpenGL ES 1.1.

