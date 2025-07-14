

- Core Image
- CIContext
-  createCGLayer(with:info:) Deprecated

Instance Method

# createCGLayer(with:info:)

Creates a CGLayer object from the provided parameters.

macOS 10.4–10.11Deprecated

``` source
func createCGLayer(
    with size: CGSize,
    info: CFDictionary?
) -> CGLayer?
```

## Parameters 

`size`  

The size, in default user space units, of the layer relative to the graphics context.

`d`  

A dictionary, which is passed to `CGLayerCreateWithContext` as the `auxiliaryInfo` parameter. Pass `NULL` because this parameter is reserved for future use.

## Return Value

A CGLayer object.

## Discussion

After calling this method, Core Image draws content into the CGLayer object. Core Image creates a CGLayer object by calling the Quartz 2D function init(_:size:auxiliaryInfo:), whose prototype is:

CGLayerRef CGLayerCreateWithContext (
   CGContextRef context,
   CGSize size,
   CFDictionaryRef auxiliaryInfo
);

Core Image passes the `CIContext` object as the `context` parameter, the size as the `size` parameter, and the dictionary as the `auxiliaryInfo` parameter. For more information on CGLayer objects, see Quartz 2D Programming Guide and `CGLayer`.

## See Also

### Deprecated

init(cglContext: CGLContextObj, pixelFormat: CGLPixelFormatObj?, colorSpace: CGColorSpace?, options: [CIContextOption : Any]?)

Creates a Core Image context from a CGL context, using the specified options, color space, and pixel format object.

Deprecated

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

### Related Documentation

+ imageWithCGLayer:

Creates and returns an image object from the contents supplied by a `CGLayer` object.

+ imageWithCGLayer:options:

Creates and returns an image object from the contents supplied by a `CGLayer` object, using the specified options.

