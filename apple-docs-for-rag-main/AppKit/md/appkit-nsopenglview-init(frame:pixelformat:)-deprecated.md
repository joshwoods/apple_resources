

- AppKit
- NSOpenGLView
-  init(frame:pixelFormat:) Deprecated

Initializer

# init(frame:pixelFormat:)

Returns an `NSOpenGLView` object initialized with the specified frame rectangle and pixel format.

macOS 10.0–10.14Deprecated

``` source
@MainActor
init?(
    frame frameRect: NSRect,
    pixelFormat format: NSOpenGLPixelFormat?
)
```

Deprecated

Please use MTKView instead.

## Parameters 

`frameRect`  

The frame rectangle for the view, specified in the coordinate system of its parent view.

`format`  

The pixel format to use when creating the view’s `NSOpenGLContext` object.

## Return Value

An initialized `NSOpenGLView` object, or `nil` if the object could not be initialized.

## See Also

### Related Documentation

class func defaultPixelFormat() -> NSOpenGLPixelFormat

Returns a default NSOpenGLPixelFormat object.

Deprecated

Cocoa Drawing Guide

