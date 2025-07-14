

- Metal
- MTLArgumentEncoder
-  setBuffers(\_:offsets:range:) 

Instance Method

# setBuffers(\_:offsets:range:)

Encodes references to an array of buffers into the argument buffer.

iOS 11.0+iPadOS 11.0+Mac CatalystmacOS 10.13+tvOS 11.0+visionOS

``` source
func setBuffers(
    _ buffers: [(any MTLBuffer)?],
    offsets: [Int],
    range: Range
)
```

## Parameters 

`buffers`  

An array of buffers the method encodes.

`offsets`  

An array of byte offsets for each element in `buffers`.

`range`  

A range of indices within the argument buffer for each element in `buffers`. The values correspond to either the index IDs of declarations in Metal Shading Language (MSL) or the index property of MTLArgumentDescriptor instances.

## See Also

### Encoding Buffers

func setBuffer((any MTLBuffer)?, offset: Int, index: Int)

Encodes a reference to a buffer into the argument buffer.

**Required**

