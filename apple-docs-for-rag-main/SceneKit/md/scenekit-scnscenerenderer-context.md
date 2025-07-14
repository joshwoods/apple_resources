

- SceneKit
- SCNSceneRenderer
-  context 

Instance Property

# context

The OpenGL rendering context that SceneKit uses for rendering the scene.

iOSiPadOSmacOStvOS

``` source
var context: UnsafeMutableRawPointer? { get }
```

**Required**

## Discussion

In macOS, the value of this property is a Core OpenGL cglContextObj object.

In iOS, the value of this property is an EAGLContext object.

