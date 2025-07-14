

- Metal
- MTLInstanceAccelerationStructureDescriptor
-  motionTransformBufferOffset 

Instance Property

# motionTransformBufferOffset

The offset, in bytes, to the descripton of the first motion transform.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var motionTransformBufferOffset: Int { get set }
```

## See Also

### Specifying Motion Data

var motionTransformCount: Int

The number of motion transforms in the motion transform buffer.

var motionTransformBuffer: (any MTLBuffer)?

A buffer that contains descriptions of each motion transform in the acceleration structure.

