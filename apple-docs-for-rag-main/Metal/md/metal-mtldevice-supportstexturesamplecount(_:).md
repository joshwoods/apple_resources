

- Metal
- MTLDevice
-  supportsTextureSampleCount(\_:) 

Instance Method

# supportsTextureSampleCount(\_:)

Returns a Boolean value that indicates whether the GPU can sample a texture with a specific number of sample points.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func supportsTextureSampleCount(_ sampleCount: Int) -> Bool
```

**Required**

## Parameters 

`sampleCount`  

The number of points a GPU can sample from a texture.

## Mentioned in 

Positioning Samples Programmatically

## Discussion

The number of points the GPU can sample a texture varies by device:

| Sample count | Devices |
|----|----|
| 1 | All devices |
| 2 | All iOS devices  All tvOS devices  Some macOS devices |
| 4 | All devices |
| 8 | Some macOS devices |

Consider a GPU device’s limitations for sample count by checking MTLTexture`.`sampleCount when configuring these properties:

- MTLTextureDescriptor`.`sampleCount

- MTLRenderPipelineDescriptor`.`rasterSampleCount

- MTLTileRenderPipelineDescriptor`.`rasterSampleCount

- MTLMeshRenderPipelineDescriptor`.`rasterSampleCount

- MTKView`.`sampleCount

## See Also

### Creating Samplers

func makeSamplerState(descriptor: MTLSamplerDescriptor) -> (any MTLSamplerState)?

Creates a sampler state instance.

**Required**

func getDefaultSamplePositions(sampleCount: Int) -> [MTLSamplePosition]

Returns the default sample locations based on the number of samples.

