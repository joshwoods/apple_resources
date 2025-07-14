

- Metal
- MTLArgumentEncoder
-  setSamplerStates(\_:range:) 

Instance Method

# setSamplerStates(\_:range:)

Encodes an array of samplers into the argument buffer.

iOS 11.0+iPadOS 11.0+Mac CatalystmacOS 10.13+tvOS 11.0+visionOS

``` source
func setSamplerStates(
    _ samplers: [(any MTLSamplerState)?],
    range: Range
)
```

## Parameters 

`samplers`  

An array of samplers the method encodes.

`range`  

A range of indices within the argument buffer for each element in `samplers`. The values correspond to either the index IDs of declarations in Metal Shading Language (MSL) or the index property of MTLArgumentDescriptor instances.

## See Also

### Encoding Samplers

func setSamplerState((any MTLSamplerState)?, index: Int)

Encodes a sampler into the argument buffer.

**Required**

