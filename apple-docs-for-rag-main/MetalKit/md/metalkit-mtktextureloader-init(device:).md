

- MetalKit
- MTKTextureLoader
-  init(device:) 

Initializer

# init(device:)

Initializes a new texture loader object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(device: any MTLDevice)
```

## Parameters 

`device`  

The Metal device to create Metal textures with.

## Return Value

An initialized texture loader object.

## See Also

### Creating a Texture Loader

var device: any MTLDevice

The device object that the texture loader uses to create textures.

