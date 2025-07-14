

- Metal
- MTLFunction
-  makeArgumentEncoder(bufferIndex:reflection:) Deprecated

Instance Method

# makeArgumentEncoder(bufferIndex:reflection:)

Creates an argument encoder and returns reflection information for an argument buffer that’s one of this function’s arguments

iOS 11.0–16.0DeprecatediPadOS 11.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.13–13.0DeprecatedtvOS 11.0–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func makeArgumentEncoder(
    bufferIndex: Int,
    reflection: AutoreleasingUnsafeMutablePointer?
) -> any MTLArgumentEncoder
```

**Required**

Deprecated

Use the makeArgumentEncoder(bufferBinding:) method of an MTLDevice instance.

## Parameters 

`bufferIndex`  

The index of an argument buffer in the function’s argument list. This method fails if the specified index doesn’t correspond to an argument buffer.

`reflection`  

A pointer that Metal populates with the function reflection data in the argument buffer at `bufferIndex`.

## Discussion

Resources encoded into an argument buffer by the MTLArgumentEncoder object must match the structure of the argument buffer located at the function’s specified buffer index.

## See Also

### Creating Argument Encoders

func makeArgumentEncoder(bufferIndex: Int) -> any MTLArgumentEncoder

Creates an argument encoder for an argument buffer that’s one of this function’s arguments.

**Required**

