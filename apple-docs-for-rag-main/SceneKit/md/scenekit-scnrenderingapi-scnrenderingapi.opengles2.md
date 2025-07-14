

- SceneKit
- SCNRenderingAPI
-  SCNRenderingAPI.openGLES2 

Case

# SCNRenderingAPI.openGLES2

Use the OpenGL ES 2.0 API for SceneKit rendering in iOS.

iOS 9.0+iPadOS 9.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case openGLES2
```

## Discussion

This option is available on all iOS devices supporting SceneKit. If you request the Metal rendering API for an SCNView object on a device that does not support Metal, SceneKit falls back to the OpenGL ES 2.0 API.

## See Also

### Constants

case metal

Use the Metal framework for SceneKit rendering.

case openGLLegacy

Use the Legacy OpenGL API for SceneKit rendering in macOS.

case openGLCore32

Use the OpenGL 3.2 Core Profile API for SceneKit rendering in macOS.

case openGLCore41

Use the OpenGL 4.1 Core Profile API for SceneKit rendering in macOS.

