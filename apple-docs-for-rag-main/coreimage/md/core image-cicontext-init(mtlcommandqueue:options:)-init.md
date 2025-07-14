

- Core Image
- CIContext
-  init(mtlCommandQueue:options:) 

Initializer

# init(mtlCommandQueue:options:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
init(
    mtlCommandQueue commandQueue: any MTLCommandQueue,
    options: [CIContextOption : Any]? = nil
)
```

## See Also

### Creating a Context for GPU-Based Rendering

init(mtlDevice: any MTLDevice)

Creates a Core Image context using the specified Metal device.

init(mtlDevice: any MTLDevice, options: [CIContextOption : Any]?)

Creates a Core Image context using the specified Metal device and options.

init(mtlCommandQueue: any MTLCommandQueue)

