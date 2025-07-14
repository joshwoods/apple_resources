

- Metal
- MTLRenderCommandEncoder
-  setMeshSamplerStates(\_:lodMinClamps:lodMaxClamps:range:) 

Instance Method

# setMeshSamplerStates(\_:lodMinClamps:lodMaxClamps:range:)

Assigns multiple sampler states and clamp values to a range of entries in the mesh shader argument table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS

``` source
func setMeshSamplerStates(
    _ samplers: [(any MTLSamplerState)?],
    lodMinClamps: [Float],
    lodMaxClamps: [Float],
    range: Range
)
```

## Parameters 

`samplers`  

An array of MTLSamplerState instances the command assigns to entries in the mesh shader argument table for sampler states.

`lodMinClamps`  

An array of floating-point values. Each element is the smallest level of detail value a mesh shader can use when it samples a texture with the corresponding element in `samplers`.

`lodMaxClamps`  

An array of floating-point values. Each element is the largest level of detail value a mesh shader can use when it samples a texture with the corresponding element in `samplers`.

`range`  

A span of integers that represent the entries in the mesh shader argument table for sampler states. Each entry stores a record of the corresponding element in `samplers`.

## Discussion

Each element of the method’s `lodMinClamps` and `lodMaxClamps` parameters overrides the default values for the corresponding sampler in `samplers`. You can set a sampler’s default values by configuring the lodMinClamp and lodMaxClamp properties of MTLSamplerDescriptor before you create the sampler.

By default, the sampler state at each index is `nil`.

Note

The Objective-C version of this method is setMeshSamplerStates:lodMinClamps:lodMaxClamps:withRange:.

## See Also

### Assigning Sampler States for Mesh Shaders

func setMeshSamplerState((any MTLSamplerState)?, index: Int)

Assigns a sampler state to an entry in the mesh shader argument table.

**Required**

func setMeshSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the mesh shader argument table.

**Required**

func setMeshSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Assigns multiple sampler states to a range of entries in the mesh shader argument table.

