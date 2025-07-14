

- Metal
- MTLRenderCommandEncoder
-  setTileSamplerState(\_:index:) 

Instance Method

# setTileSamplerState(\_:index:)

Assigns a sampler state to an entry in the tile shader argument table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func setTileSamplerState(
    _ sampler: (any MTLSamplerState)?,
    index: Int
)
```

**Required**

## Parameters 

`sampler`  

An MTLSamplerState instance the command assigns to an entry in the tile shader argument table for sampler states.

`index`  

An integer that represents the entry in the tile shader argument table for sampler states that stores a record of `sampler`.

## Discussion

By default, the sampler state at each index is `nil`.

## See Also

### Assigning Sampler States

func setTileSamplerState((any MTLSamplerState)?, lodMinClamp: Float, lodMaxClamp: Float, index: Int)

Assigns a sampler state and clamp values to an entry in the tile shader argument table.

**Required**

func setTileSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Assigns multiple sampler states to a range of entries in the tile shader argument table.

func setTileSamplerStates([(any MTLSamplerState)?], lodMinClamps: [Float], lodMaxClamps: [Float], range: Range&lt;Int>)

Assigns multiple sampler states and clamp values to a range of entries in the tile shader argument table.

