

- Metal
- MTLInstanceAccelerationStructureDescriptor
-  motionTransformBuffer 

Instance Property

# motionTransformBuffer

A buffer that contains descriptions of each motion transform in the acceleration structure.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var motionTransformBuffer: (any MTLBuffer)? { get set }
```

## See Also

### Specifying Motion Data

var motionTransformCount: Int

The number of motion transforms in the motion transform buffer.

var motionTransformBufferOffset: Int

The offset, in bytes, to the descripton of the first motion transform.

