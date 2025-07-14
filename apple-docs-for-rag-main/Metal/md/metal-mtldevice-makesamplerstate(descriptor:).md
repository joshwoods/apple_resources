

- Metal
- MTLDevice
-  makeSamplerState(descriptor:) 

Instance Method

# makeSamplerState(descriptor:)

Creates a sampler state instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeSamplerState(descriptor: MTLSamplerDescriptor) -> (any MTLSamplerState)?
```

**Required**

## Parameters 

`descriptor`  

An MTLSamplerDescriptor instance.

## Return Value

A new MTLSamplerState instance if the method completed successfully; otherwise `nil`.

## See Also

### Creating Samplers

func supportsTextureSampleCount(Int) -> Bool

Returns a Boolean value that indicates whether the GPU can sample a texture with a specific number of sample points.

**Required**

func getDefaultSamplePositions(sampleCount: Int) -> [MTLSamplePosition]

Returns the default sample locations based on the number of samples.

