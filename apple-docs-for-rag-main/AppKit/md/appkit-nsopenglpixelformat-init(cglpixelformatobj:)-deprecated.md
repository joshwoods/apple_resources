

- AppKit
- NSOpenGLPixelFormat
-  init(cglPixelFormatObj:) Deprecated

Initializer

# init(cglPixelFormatObj:)

Returns an OpenGL pixel format object initialized with using an existing CGL pixel format object.

macOS 10.6–10.14Deprecated

``` source
init?(cglPixelFormatObj format: CGLPixelFormatObj)
```

## Parameters 

`format`  

An existing CGL pixel format object.

## Return Value

An intialized NSOpenGLPixelFormat object that wraps the CGL pixel format object.

## Discussion

If your application already has a low-level CGL pixel format object, you can create an NSOpenGLPixelFormat object to wrap it by calling this initializer. The NSOpenGLPixelFormat object retains the CGL pixel format object by calling the `CGLRetainPixelFormat(_:)` function.

Your application should not call `CGLDestroyPixelFormat(_:)` to dispose of the CGL pixel format object. Instead, your application should call `CGLReleasePixelFormat(_:)` to decrement its reference count.

## See Also

### Related Documentation

Cocoa Drawing Guide

### Creating an OpenGL Pixel Format

convenience init?(attributes: UnsafePointer&lt;NSOpenGLPixelFormatAttribute>)

Returns an OpenGL pixel format object initialized with specified pixel format attributes.

Deprecated

