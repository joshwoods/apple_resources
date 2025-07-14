

- AppKit
- NSOpenGLContext
-  init(cglContextObj:) Deprecated

Initializer

# init(cglContextObj:)

Initializes and returns an OpenGL context object using an existing CGL context.

macOS 10.6–10.14Deprecated

``` source
init?(cglContextObj context: CGLContextObj)
```

## Parameters 

`context`  

The CGL context to wrap inside the NSOpenGLContext object.

## Return Value

An initialized context.

## Discussion

If your application already has a CGL context, you can wrap a NSOpenGLContext object around it using this method. This method retains the CGL context by calling `CGLRetainContext(_:)`.

Only one NSOpenGLContext object can wrap a specific context.

Your application should not call `CGLDestroyContext(_:)` to dispose of the CGL context. Instead, your application should call `CGLReleaseContext(_:)` to decrement its reference count.

## See Also

### Creating Contexts

init?(format: NSOpenGLPixelFormat, share: NSOpenGLContext?)

Returns an OpenGL context object initialized with the specified pixel format information.

Deprecated

