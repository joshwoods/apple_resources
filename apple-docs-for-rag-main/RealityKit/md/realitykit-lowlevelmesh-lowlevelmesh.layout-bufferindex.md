

- RealityKit
- LowLevelMesh
- LowLevelMesh.Layout
-  bufferIndex 

Instance Property

# bufferIndex

The index of the buffer to use for this layout.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var bufferIndex: Int
```

## Discussion

Most usage scenarios only use one buffer. Use a buffer index that is less than vertexBufferCount.

## See Also

### Describing a low-level mesh layout

var bufferOffset: Int

The byte offset into the buffer for the first byte of this layout.

var bufferStride: Int

The distance, in bytes, between consecutive vertices for attributes using this layout.

