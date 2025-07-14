

- Metal
- MTLArgumentEncoder
-  setArgumentBuffer(\_:offset:) 

Instance Method

# setArgumentBuffer(\_:offset:)

Specifies the position in a buffer where the encoder writes argument data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func setArgumentBuffer(
    _ argumentBuffer: (any MTLBuffer)?,
    offset: Int
)
```

**Required**

## Parameters 

`argumentBuffer`  

The destination buffer that represents an argument buffer.

`offset`  

The byte offset of the buffer.

## See Also

### Creating an Argument Buffer

func setArgumentBuffer((any MTLBuffer)?, startOffset: Int, arrayElement: Int)

Specifies an array element within a buffer where the encoder writes argument data.

**Required**

var encodedLength: Int

The number of bytes required to store the encoded resources of an argument buffer.

**Required**

