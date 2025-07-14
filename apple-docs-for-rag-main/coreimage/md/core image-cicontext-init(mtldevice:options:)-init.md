

- Core Image
- CIContext
-  init(mtlDevice:options:) 

Initializer

# init(mtlDevice:options:)

Creates a Core Image context using the specified Metal device and options.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    mtlDevice device: any MTLDevice,
    options: [CIContextOption : Any]? = nil
)
```

## Parameters 

`device`  

The Metal device object to use for rendering.

`options`  

A dictionary that contains options for creating a `CIContext` object. You can pass any of the keys defined in `Context Options` along with the appropriate value.

## Return Value

A Core Image context.

## Discussion

Use this method to choose a specific Metal device for rendering when a system contains multiple Metal devices. To create a Metal-based context using the system’s default Metal device, use the init(options:) method.

## See Also

### Creating a Context for GPU-Based Rendering

init(mtlDevice: any MTLDevice)

Creates a Core Image context using the specified Metal device.

init(mtlCommandQueue: any MTLCommandQueue)

init(mtlCommandQueue: any MTLCommandQueue, options: [CIContextOption : Any]?)

