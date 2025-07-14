

- MetalFX
- MTLFXTemporalScalerDescriptor
-  makeTemporalScaler(device:) 

Instance Method

# makeTemporalScaler(device:)

Creates a temporal scaler instance from this descriptor’s current property values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
func makeTemporalScaler(device: any MTLDevice) -> (any MTLFXTemporalScaler)?
```

## Parameters 

`device`  

An MTLDevice instance that represents the GPU that applies the temporal scaling effect.

