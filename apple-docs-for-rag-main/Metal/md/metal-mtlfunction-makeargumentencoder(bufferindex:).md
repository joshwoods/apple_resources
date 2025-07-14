

- Metal
- MTLFunction
-  makeArgumentEncoder(bufferIndex:) 

Instance Method

# makeArgumentEncoder(bufferIndex:)

Creates an argument encoder for an argument buffer that’s one of this function’s arguments.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func makeArgumentEncoder(bufferIndex: Int) -> any MTLArgumentEncoder
```

**Required**

## Parameters 

`bufferIndex`  

The index of an argument buffer in the function’s argument list. This method fails if the specified index doesn’t correspond to an argument buffer.

## Discussion

Resources encoded into an argument buffer by the MTLArgumentEncoder object must match the structure of the argument buffer located at the specified buffer index. If you want to interpret a regular structure as an argument buffer, at least one of the members of the structure must have an `[[id(n)]]` attribute.

## See Also

### Creating Argument Encoders

func makeArgumentEncoder(bufferIndex: Int, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedArgument?>?) -> any MTLArgumentEncoder

Creates an argument encoder and returns reflection information for an argument buffer that’s one of this function’s arguments

**Required**

Deprecated

