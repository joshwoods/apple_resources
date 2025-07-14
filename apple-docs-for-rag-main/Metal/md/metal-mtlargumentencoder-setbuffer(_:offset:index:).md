

- Metal
- MTLArgumentEncoder
-  setBuffer(\_:offset:index:) 

Instance Method

# setBuffer(\_:offset:index:)

Encodes a reference to a buffer into the argument buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func setBuffer(
    _ buffer: (any MTLBuffer)?,
    offset: Int,
    index: Int
)
```

**Required**

## Parameters 

`buffer`  

A buffer the method encodes.

`offset`  

A byte offset for `buffer`.

`index`  

The index of a buffer within the argument buffer. The value corresponds to either the index ID of a declaration in Metal Shading Language (MSL) or the index property of an MTLArgumentDescriptor instance.

## See Also

### Encoding Buffers

func setBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Encodes references to an array of buffers into the argument buffer.

