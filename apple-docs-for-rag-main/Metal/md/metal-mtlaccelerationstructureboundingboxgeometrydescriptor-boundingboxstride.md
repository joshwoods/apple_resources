

- Metal
- MTLAccelerationStructureBoundingBoxGeometryDescriptor
-  boundingBoxStride 

Instance Property

# boundingBoxStride

The stride, in bytes, between bounding boxes in the buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var boundingBoxStride: Int { get set }
```

## Discussion

The stride must be at least 24 bytes, and must be a multiple of 4 bytes. The default value is 24 bytes.

## See Also

### Specifying Bounding Boxes Data

var boundingBoxBuffer: (any MTLBuffer)?

A buffer that contains bounding box data.

var boundingBoxBufferOffset: Int

The offset, in bytes, to the first bounding box in the buffer.

