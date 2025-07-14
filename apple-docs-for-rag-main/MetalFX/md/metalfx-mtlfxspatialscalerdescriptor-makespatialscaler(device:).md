

- MetalFX
- MTLFXSpatialScalerDescriptor
-  makeSpatialScaler(device:) 

Instance Method

# makeSpatialScaler(device:)

Creates a spatial scaler instance from this descriptor’s current property values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func makeSpatialScaler(device: any MTLDevice) -> (any MTLFXSpatialScaler)?
```

## Parameters 

`device`  

An MTLDevice instance that represents the GPU that applies the spatial scaler.

