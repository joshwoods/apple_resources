

- Core Image
- CIContext
-  init(eaglContext:options:) Deprecated

Initializer

# init(eaglContext:options:)

Creates a Core Image context from an EAGL context using the specified options.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
init(
    eaglContext: EAGLContext,
    options: [CIContextOption : Any]? = nil
)
```

## Parameters 

`eaglContext`  

The EAGL context to render to.

`options`  

A dictionary that contains options for creating a `CIContext` object. You can pass any of the keys defined in `Context Options` along with the appropriate value.

## Return Value

A Core Image context that targets OpenGL ES.

## Discussion

The OpenGL ES context must support OpenGL ES 2.0. All drawing performed using the methods listed in Drawing Images is rendered directly into the context.

## See Also

### Deprecated

init(cglContext: CGLContextObj, pixelFormat: CGLPixelFormatObj?, colorSpace: CGColorSpace?, options: [CIContextOption : Any]?)

Creates a Core Image context from a CGL context, using the specified options, color space, and pixel format object.

Deprecated

init(eaglContext: EAGLContext)

Creates a Core Image context from an EAGL context.

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

