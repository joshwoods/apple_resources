

- Metal
- MTLRenderCommandEncoder
-  setTileSamplerStates(\_:range:) 

Instance Method

# setTileSamplerStates(\_:range:)

Assigns multiple sampler states to a range of entries in the tile shader argument table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS

``` source
func setTileSamplerStates(
    _ samplers: [(any MTLSamplerState)?],
    range: Range
)
```

## Parameters 

`samplers`  

An array of MTLSamplerState instances the command assigns to entries in the tile shader argument table for sampler states.

`range`  

A span of integers that represent the entries in the tile shader argument table for sampler states. Each entry stores a record of the corresponding element in `samplers`.

## Discussion

By default, the sampler state at each index is `nil`.

Note

The Objective-C version of this method is setTileSamplerStates:withRange:.

## See Also

### Assigning Sampler States

func setTileSamplerState((any MTLSamplerState)?, index: Int)

Assigns a sampler state to an entry in the tile shader argument table.

**Required**

func setTileSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the tile shader argument table.

**Required**

func setTileSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Assigns multiple sampler states and clamp values to a range of entries in the tile shader argument table.

