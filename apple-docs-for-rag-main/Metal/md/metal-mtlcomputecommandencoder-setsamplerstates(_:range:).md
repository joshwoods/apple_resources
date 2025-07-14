

- Metal
- MTLComputeCommandEncoder
-  setSamplerStates(\_:range:) 

Instance Method

# setSamplerStates(\_:range:)

Encodes multiple texture samplers to the sampler argument table, allowing compute kernels to use them for sampling textures on the GPU.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.11+tvOS 8.0+visionOS

``` source
func setSamplerStates(
    _ samplers: [(any MTLSamplerState)?],
    range: Range
)
```

## Parameters 

`samplers`  

An array of MTLSamplerState instance to bind to the sampler argument table.

`range`  

The sampler table indicies to bind each of the `samplers` to, in the order they appear.

## Discussion

Warning

This method requires that the number of instances in `samplers` be the same as the length of `range`.

## See Also

### Encoding Texture Sampler States

func setSamplerState((any MTLSamplerState)?, index: Int)

Encodes a texture sampler, allowing compute kernels to use it for sampling textures on the GPU.

**Required**

func setSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Encodes a texture sampler with a custom level of detail clamping, allowing compute kernels to use it for sampling textures on the GPU.

**Required**

func setSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Encodes multiple texture samplers for the compute function, specifying clamp values for the level of detail of each sampler.

