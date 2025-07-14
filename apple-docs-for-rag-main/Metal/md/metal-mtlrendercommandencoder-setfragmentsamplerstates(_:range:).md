

- Metal
- MTLRenderCommandEncoder
-  setFragmentSamplerStates(\_:range:) 

Instance Method

# setFragmentSamplerStates(\_:range:)

Assigns multiple sampler states to a range of entries in the fragment shader argument table.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.11+tvOS 8.0+visionOS

``` source
func setFragmentSamplerStates(
    _ samplers: [(any MTLSamplerState)?],
    range: Range
)
```

## Parameters 

`samplers`  

An array of MTLSamplerState instances the command assigns to entries in the fragment shader argument table for sampler states.

`range`  

A span of integers that represent the entries in the fragment shader argument table for sampler states. Each entry stores a record of the corresponding element in `samplers`.

## Discussion

By default, the sampler state at each index is `nil`.

Note

The Objective-C version of this method is setFragmentSamplerStates:withRange:.

## See Also

### Assigning Sampler States

func setFragmentSamplerState((any MTLSamplerState)?, index: Int)

Assigns a sampler state to an entry in the fragment shader argument table.

**Required**

func setFragmentSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the fragment shader argument table.

**Required**

func setFragmentSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Assigns multiple sampler states and clamp values to a range of entries in the fragment shader argument table.

