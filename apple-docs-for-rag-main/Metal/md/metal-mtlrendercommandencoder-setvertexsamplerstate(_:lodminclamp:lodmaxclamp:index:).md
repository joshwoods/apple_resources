

- Metal
- MTLRenderCommandEncoder
-  setVertexSamplerState(\_:lodMinClamp:lodMaxClamp:index:) 

Instance Method

# setVertexSamplerState(\_:lodMinClamp:lodMaxClamp:index:)

Assigns a sampler state and clamp values to an entry in the vertex shader argument table.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setVertexSamplerState(
    _ sampler: (any MTLSamplerState)?,
    lodMinClamp: Float,
    lodMaxClamp: Float,
    index: Int
)
```

**Required**

## Parameters 

`sampler`  

An MTLSamplerState instance the command assigns to an entry in the vertex shader argument table for sampler states.

`lodMinClamp`  

The smallest level of detail value a vertex shader can use when it samples a texture.

`lodMaxClamp`  

The largest level of detail value a vertex shader can use when it samples a texture.

`index`  

An integer that represents the entry in the vertex shader argument table for sampler states that stores a record of `sampler`.

## Discussion

The method’s `lodMinClamp` and `lodMaxClamp` parameters override the default values for `sampler`. You can set the sampler’s default values by configuring the lodMinClamp and lodMaxClamp properties of MTLSamplerDescriptor before you create the sampler.

By default, the sampler state at each index is `nil`.

## See Also

### Assigning Sampler States

func setVertexSamplerState((any MTLSamplerState)?, index: Int)

Assigns a sampler state to an entry in the vertex shader argument table.

**Required**

func setVertexSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Assigns multiple sampler states to a range of entries in the vertex shader argument table.

func setVertexSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Assigns multiple sampler states and clamp values to a range of entries in the vertex shader argument table.

