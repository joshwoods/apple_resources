

- Core Image
- CIContext
-  init(forOfflineGPUAt:colorSpace:options:sharedContext:) Deprecated

Initializer

# init(forOfflineGPUAt:colorSpace:options:sharedContext:)

Creates an OpenGL-based Core Image context using a GPU that is not currently driving a display, with the specified options.

macOS 10.10–10.14Deprecated

``` source
init?(
    forOfflineGPUAt index: UInt32,
    colorSpace: CGColorSpace?,
    options: [CIContextOption : Any]? = nil,
    sharedContext: CGLContextObj?
)
```

## Parameters 

`index`  

The index of the offline GPU with which to create the context; a number between zero and the value returned by the offlineGPUCount() method.

`colorSpace`  

A color space object encapsulating color space information that is used to specify how color values are interpreted.

`options`  

A dictionary that contains options for creating a `CIContext` object. You can pass any of the keys defined in `Context Options` along with the appropriate value.

`sharedContext`  

A CGL context with which to share OpenGL resources, obtained by calling the CGL function `CGLCreateContext(_:_:_:)`. Pass `NULL` to use a context that does not share OpenGL resources.

## Return Value

A Core Image context.

## Discussion

GPU devices that are not currently being used to drive a display can be used for Core Image rendering. Use the offlineGPUCount() method to determine whether any such GPUs are available.

To create a Metal-based Core Image context using an offline GPU, use the MTLCopyAllDevices() function to list Metal devices, then choose a device without a display to pass to the init(mtlDevice:) method.

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

func createCGLayer(with: CGSize, info: CFDictionary?) -> CGLayer?

Creates a CGLayer object from the provided parameters.

Deprecated

