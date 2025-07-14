

- Core Image
- CIContext
-  init(forOfflineGPUAt:) Deprecated

Initializer

# init(forOfflineGPUAt:)

Creates an OpenGL-based Core Image context using a GPU that is not currently driving a display.

macOS 10.10–10.14Deprecated

``` source
init?(forOfflineGPUAt index: UInt32)
```

## Parameters 

`index`  

The index of the offline GPU with which to create the context; a number between zero and the value returned by the offlineGPUCount() method.

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

init?(forOfflineGPUAt: UInt32, colorSpace: CGColorSpace?, options: [CIContextOption : Any]?, sharedContext: CGLContextObj?)

Creates an OpenGL-based Core Image context using a GPU that is not currently driving a display, with the specified options.

Deprecated

func createCGLayer(with: CGSize, info: CFDictionary?) -> CGLayer?

Creates a CGLayer object from the provided parameters.

Deprecated

