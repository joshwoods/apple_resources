

- Metal
- MTLComputeCommandEncoder
-  setSamplerState(\_:lodMinClamp:lodMaxClamp:index:) 

Instance Method

# setSamplerState(\_:lodMinClamp:lodMaxClamp:index:)

Encodes a texture sampler with a custom level of detail clamping, allowing compute kernels to use it for sampling textures on the GPU.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setSamplerState(
    _ sampler: (any MTLSamplerState)?,
    lodMinClamp: Float,
    lodMaxClamp: Float,
    index: Int
)
```

**Required**

## Parameters 

`sampler`  

An MTLSamplerState instance to bind to the sampler argument table.

`lodMinClamp`  

The minimum level of detail used when sampling a texture.

`lodMaxClamp`  

The maximum level of detail used when sampling a texture.

`index`  

The index in the sampler argument table to bind the sampler to.

## Discussion

Calling this method ignores the lodMinClamp and lodMaxClamp properties of the sampler, using the provided levels of detail instead.

## See Also

### Encoding Texture Sampler States

func setSamplerState((any MTLSamplerState)?, index: Int)

Encodes a texture sampler, allowing compute kernels to use it for sampling textures on the GPU.

**Required**

func setSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Encodes multiple texture samplers to the sampler argument table, allowing compute kernels to use them for sampling textures on the GPU.

func setSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Encodes multiple texture samplers for the compute function, specifying clamp values for the level of detail of each sampler.

