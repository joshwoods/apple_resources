

- Metal
- MTLArgumentEncoder
-  setSamplerState(\_:index:) 

Instance Method

# setSamplerState(\_:index:)

Encodes a sampler into the argument buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func setSamplerState(
    _ sampler: (any MTLSamplerState)?,
    index: Int
)
```

**Required**

## Parameters 

`sampler`  

A sampler the method encodes.

`index`  

The index of a sampler within the argument buffer. The value corresponds to either the index ID of a declaration in Metal Shading Language (MSL) or the index property of an MTLArgumentDescriptor instance.

## See Also

### Encoding Samplers

func setSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Encodes an array of samplers into the argument buffer.

