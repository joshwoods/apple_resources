

- Metal
- MTLArgumentEncoder
-  setArgumentBuffer(\_:startOffset:arrayElement:) 

Instance Method

# setArgumentBuffer(\_:startOffset:arrayElement:)

Specifies an array element within a buffer where the encoder writes argument data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func setArgumentBuffer(
    _ argumentBuffer: (any MTLBuffer)?,
    startOffset: Int,
    arrayElement: Int
)
```

**Required**

## Parameters 

`argumentBuffer`  

The destination buffer that represents an argument buffer.

`startOffset`  

The starting byte offset of the buffer data.

`arrayElement`  

The desired element of the argument buffer array targeted by encoding.

## See Also

### Creating an Argument Buffer

func setArgumentBuffer((any MTLBuffer)?, offset: Int)

Specifies the position in a buffer where the encoder writes argument data.

**Required**

var encodedLength: Int

The number of bytes required to store the encoded resources of an argument buffer.

**Required**

