

- SceneKit
- SCNRenderingAPI
-  SCNRenderingAPI.openGLLegacy 

Case

# SCNRenderingAPI.openGLLegacy

Use the Legacy OpenGL API for SceneKit rendering in macOS.

macOS 10.11+

``` source
case openGLLegacy
```

## Discussion

This option is available on all macOS systems supporting SceneKit. If you request the Metal rendering API for an SCNView object on a system that does not support Metal, SceneKit falls back to the Legacy OpenGL API.

## See Also

### Constants

case metal

Use the Metal framework for SceneKit rendering.

case openGLES2

Use the OpenGL ES 2.0 API for SceneKit rendering in iOS.

case openGLCore32

Use the OpenGL 3.2 Core Profile API for SceneKit rendering in macOS.

case openGLCore41

Use the OpenGL 4.1 Core Profile API for SceneKit rendering in macOS.

