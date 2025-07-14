

- Metal
- MTLAccelerationStructureBoundingBoxGeometryDescriptor
-  boundingBoxBufferOffset 

Instance Property

# boundingBoxBufferOffset

The offset, in bytes, to the first bounding box in the buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var boundingBoxBufferOffset: Int { get set }
```

## Discussion

The offset must be a multiple of boundingBoxStride, and must be aligned to the platform’s buffer offset alignment.

## See Also

### Specifying Bounding Boxes Data

var boundingBoxBuffer: (any MTLBuffer)?

A buffer that contains bounding box data.

var boundingBoxStride: Int

The stride, in bytes, between bounding boxes in the buffer.

