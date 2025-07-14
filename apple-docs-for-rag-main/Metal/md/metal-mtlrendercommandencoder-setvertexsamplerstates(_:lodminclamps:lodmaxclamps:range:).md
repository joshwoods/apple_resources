

- Metal
- MTLRenderCommandEncoder
-  setVertexSamplerStates(\_:lodMinClamps:lodMaxClamps:range:) 

Instance Method

# setVertexSamplerStates(\_:lodMinClamps:lodMaxClamps:range:)

Assigns multiple sampler states and clamp values to a range of entries in the vertex shader argument table.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.11+tvOS 8.0+visionOS

``` source
func setVertexSamplerStates(
    _ samplers: [(any MTLSamplerState)?],
    lodMinClamps: [Float],
    lodMaxClamps: [Float],
    range: Range
)
```

## Parameters 

`samplers`  

An array of MTLSamplerState instances the command assigns to entries in the vertex shader argument table for sampler states.

`lodMinClamps`  

An array of floating-point values. Each element is the smallest level of detail value a vertex shader can use when it samples a texture with the corresponding element in `samplers`.

`lodMaxClamps`  

An array of floating-point values. Each element is the largest level of detail value a vertex shader can use when it samples a texture with the corresponding element in `samplers`.

`range`  

A span of integers that represent the entries in the vertex shader argument table for sampler states. Each entry stores a record of the corresponding element in `samplers`.

## Discussion

Each element of the method’s `lodMinClamps` and `lodMaxClamps` parameters overrides the default values for the corresponding sampler in `samplers`. You can set a sampler’s default values by configuring the lodMinClamp and lodMaxClamp properties of MTLSamplerDescriptor before you create the sampler.

By default, the sampler state at each index is `nil`.

Note

The Objective-C version of this method is setVertexSamplerStates:lodMinClamps:lodMaxClamps:withRange:.

## See Also

### Assigning Sampler States

func setVertexSamplerState((any MTLSamplerState)?, index: Int)

Assigns a sampler state to an entry in the vertex shader argument table.

**Required**

func setVertexSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the vertex shader argument table.

**Required**

func setVertexSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Assigns multiple sampler states to a range of entries in the vertex shader argument table.

