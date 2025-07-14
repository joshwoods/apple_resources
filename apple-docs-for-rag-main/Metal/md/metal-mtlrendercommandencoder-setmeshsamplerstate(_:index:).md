

- Metal
- MTLRenderCommandEncoder
-  setMeshSamplerState(\_:index:) 

Instance Method

# setMeshSamplerState(\_:index:)

Assigns a sampler state to an entry in the mesh shader argument table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func setMeshSamplerState(
    _ sampler: (any MTLSamplerState)?,
    index: Int
)
```

**Required**

## Parameters 

`sampler`  

An MTLSamplerState instance the command assigns to an entry in the mesh shader argument table for sampler states.

`index`  

An integer that represents the entry in the mesh shader argument table for sampler states that stores a record of `sampler`.

## Discussion

By default, the sampler state at each index is `nil`.

## See Also

### Assigning Sampler States for Mesh Shaders

func setMeshSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the mesh shader argument table.

**Required**

func setMeshSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Assigns multiple sampler states to a range of entries in the mesh shader argument table.

func setMeshSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Assigns multiple sampler states and clamp values to a range of entries in the mesh shader argument table.

