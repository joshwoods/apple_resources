

- Metal
- MTLRenderCommandEncoder
-  setMeshSamplerStates(\_:range:) 

Instance Method

# setMeshSamplerStates(\_:range:)

Assigns multiple sampler states to a range of entries in the mesh shader argument table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS

``` source
func setMeshSamplerStates(
    _ samplers: [(any MTLSamplerState)?],
    range: Range
)
```

## Parameters 

`samplers`  

An array of MTLSamplerState instances the command assigns to entries in the mesh shader argument table for sampler states.

`range`  

A span of integers that represent the entries in the mesh shader argument table for sampler states. Each entry stores a record of the corresponding element in `samplers`.

## Discussion

By default, the sampler state at each index is `nil`.

Note

The Objective-C version of this method is setMeshSamplerStates:withRange:.

## See Also

### Assigning Sampler States for Mesh Shaders

func setMeshSamplerState((any MTLSamplerState)?, index: Int)

Assigns a sampler state to an entry in the mesh shader argument table.

**Required**

func setMeshSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the mesh shader argument table.

**Required**

func setMeshSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Assigns multiple sampler states and clamp values to a range of entries in the mesh shader argument table.

