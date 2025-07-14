

- Metal
- MTLRenderCommandEncoder
-  setFragmentSamplerState(\_:index:) 

Instance Method

# setFragmentSamplerState(\_:index:)

Assigns a sampler state to an entry in the fragment shader argument table.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setFragmentSamplerState(
    _ sampler: (any MTLSamplerState)?,
    index: Int
)
```

**Required**

## Parameters 

`sampler`  

An MTLSamplerState instance the command assigns to an entry in the fragment shader argument table for sampler states.

`index`  

An integer that represents the entry in the fragment shader argument table for sampler states that stores a record of `sampler`.

## Discussion

By default, the sampler state at each index is `nil`.

## See Also

### Assigning Sampler States

func setFragmentSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the fragment shader argument table.

**Required**

func setFragmentSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Assigns multiple sampler states to a range of entries in the fragment shader argument table.

func setFragmentSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Assigns multiple sampler states and clamp values to a range of entries in the fragment shader argument table.

