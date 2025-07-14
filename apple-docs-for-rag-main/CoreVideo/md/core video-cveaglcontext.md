

- Core Video
-  CVEAGLContext 

Type Alias

# CVEAGLContext

A type that resolves to an EAGLContext pointer when appropriate.

iOS 4.0+iPadOS 4.0+tvOS 9.0+visionOS 1.0+

**iOS, iPadOS, tvOS**

``` source
typealias CVEAGLContext = EAGLContext
```

**visionOS**

``` source
typealias CVEAGLContext = UnsafeMutableRawPointer
```

## Discussion

Core Video can be included in procedural C projects as well as Objective-C projects, so this type resolves to `void *` when using the former.

## See Also

### Data Types

class CVOpenGLESTextureCache

