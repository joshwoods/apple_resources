

- Metal
- MTLComputeCommandEncoder
-  setSamplerStates(\_:lodMinClamps:lodMaxClamps:range:) 

Instance Method

# setSamplerStates(\_:lodMinClamps:lodMaxClamps:range:)

Encodes multiple texture samplers for the compute function, specifying clamp values for the level of detail of each sampler.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.11+tvOS 8.0+visionOS

``` source
func setSamplerStates(
    _ samplers: [(any MTLSamplerState)?],
    lodMinClamps: [Float],
    lodMaxClamps: [Float],
    range: Range
)
```

## Parameters 

`samplers`  

A list of MTLSamplerState instances to bind to the sampler argument table.

`lodMinClamps`  

An array of minimum levels of detail to use for the corresponding sampler in `samplers`.

`lodMaxClamps`  

An array of maximum levels of detail to use for the corresponding sample in `samplers`.

`range`  

A range of indices in the sampler state argument table.

## Discussion

Important

This method requires that the lengths of `samplers`, `lodMinClamps`, and `lodMaxClamps` be the same as the length of `range`.

Calling this method ignores the lodMinClamp and lodMaxClamp properties of the samplers, using the provided levels of detail instead.

## See Also

### Encoding Texture Sampler States

func setSamplerState((any MTLSamplerState)?, index: Int)

Encodes a texture sampler, allowing compute kernels to use it for sampling textures on the GPU.

**Required**

func setSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Encodes a texture sampler with a custom level of detail clamping, allowing compute kernels to use it for sampling textures on the GPU.

**Required**

func setSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Encodes multiple texture samplers to the sampler argument table, allowing compute kernels to use them for sampling textures on the GPU.

