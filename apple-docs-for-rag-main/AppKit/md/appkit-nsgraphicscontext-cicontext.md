

- AppKit
- NSGraphicsContext
-  ciContext 

Instance Property

# ciContext

A context for Core Image objects that you can use to render into the graphics context.

macOS

``` source
var ciContext: CIContext? { get }
```

## Discussion

The CIContext object is created on demand and remains in existence for the lifetime of its owning NSGraphicsContext object. A CIContext object is an evaluation context for rendering a CIImage object through Quartz 2D or OpenGL. You use CIContextobjects in conjunction with CIFilter, CIImage, CIVector, and CIColor objects to take advantage of the built-in Core Image filters when processing images.

For more on CIContext objects and related Core Image objects, see Core Image Programming Guide.

