

- Metal
- MTLAccelerationStructureBoundingBoxGeometryDescriptor
-  boundingBoxBuffer 

Instance Property

# boundingBoxBuffer

A buffer that contains bounding box data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var boundingBoxBuffer: (any MTLBuffer)? { get set }
```

## See Also

### Specifying Bounding Boxes Data

var boundingBoxBufferOffset: Int

The offset, in bytes, to the first bounding box in the buffer.

var boundingBoxStride: Int

The stride, in bytes, between bounding boxes in the buffer.

