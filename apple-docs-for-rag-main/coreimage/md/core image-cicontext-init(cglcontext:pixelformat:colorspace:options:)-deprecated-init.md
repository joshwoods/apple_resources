

- Core Image
- CIContext
-  init(cglContext:pixelFormat:colorSpace:options:) Deprecated

Initializer

# init(cglContext:pixelFormat:colorSpace:options:)

Creates a Core Image context from a CGL context, using the specified options, color space, and pixel format object.

macOS 10.6–10.14Deprecated

``` source
init(
    cglContext cglctx: CGLContextObj,
    pixelFormat: CGLPixelFormatObj?,
    colorSpace: CGColorSpace?,
    options: [CIContextOption : Any]? = nil
)
```

## Parameters 

`ctx`  

A CGL context obtained by calling the CGL function `CGLCreateContext(_:_:_:)`.

`pf`  

A CGL pixel format object either obtained from the system or created by calling a CGL function such as `CGLChoosePixelFormat(_:_:_:)`. This parameter must be the same pixel format object used to create the CGL context. The pixel format object must be valid for the lifetime of the Core Image context. Don’t release the pixel format object until after you release the Core Image context.

`space`  

A color space object encapsulating color space information that is used to specify how color values are interpreted.

`options`  

A dictionary that contains options for creating a `CIContext` object. You can pass any of the keys defined in `Context Options` along with the appropriate value.

## Discussion

After calling this method, Core Image draws content into the surface (drawable object) attached to the CGL context. A CGL context is a macOS OpenGL context. For more information, see OpenGL Programming Guide for Mac.

When you create a `CIContext` object using a CGL context, all OpenGL states set for the CGL context affect rendering to that context. That means that coordinate and viewport transformations set on the CGL context, as well as the vertex color, affect drawing to that context.

For best results, follow these guidelines when you use Core Image to render into an OpenGL context:

- Ensure that a single unit in the coordinate space of the OpenGL context represents a single pixel in the output device.

- The Core Image coordinate space has the origin in the bottom-left corner of the screen. You should configure the OpenGL context in the same way.

- The OpenGL context blending state is respected by Core Image. If the image you want to render contains translucent pixels, it’s best to enable blending using a blend function with the parameters `GL_ONE, GL_ONE_MINUS_SRC_ALPHA`, as shown in the following code example.

Core Image manages its own internal OpenGL context that shares resources with the OpenGL context you specify. To enable resource sharing, use the following code:

let attr = [
    NSOpenGLPFAAccelerated,
    NSOpenGLPFANoRecovery,
    NSOpenGLPFAColorSize, 32,
    0
    ].map {NSOpenGLPixelFormatAttribute($0)}
let pf = NSOpenGLPixelFormat(attributes: attr)!
let myCIContext = CIContext(CGLContext: CGLGetCurrentContext(),
                            pixelFormat: pf.CGLPixelFormatObj,
                            colorSpace: CGColorSpaceCreateDeviceRGB(),
                            options: [:])

## See Also

### Deprecated

init(eaglContext: EAGLContext)

Creates a Core Image context from an EAGL context.

Deprecated

init(eaglContext: EAGLContext, options: [CIContextOption : Any]?)

Creates a Core Image context from an EAGL context using the specified options.

Deprecated

init?(forOfflineGPUAt: UInt32)

Creates an OpenGL-based Core Image context using a GPU that is not currently driving a display.

Deprecated

init?(forOfflineGPUAt: UInt32, colorSpace: CGColorSpace?, options: [CIContextOption : Any]?, sharedContext: CGLContextObj?)

Creates an OpenGL-based Core Image context using a GPU that is not currently driving a display, with the specified options.

Deprecated

func createCGLayer(with: CGSize, info: CFDictionary?) -> CGLayer?

Creates a CGLayer object from the provided parameters.

Deprecated

### Related Documentation

init(cgContext: CGContext, options: [CIContextOption : Any]?)

Creates a Core Image context from a Quartz context, using the specified options.

