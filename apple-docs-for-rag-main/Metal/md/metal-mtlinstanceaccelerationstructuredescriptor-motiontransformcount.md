

- Metal
- MTLInstanceAccelerationStructureDescriptor
-  motionTransformCount 

Instance Property

# motionTransformCount

The number of motion transforms in the motion transform buffer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var motionTransformCount: Int { get set }
```

## See Also

### Specifying Motion Data

var motionTransformBuffer: (any MTLBuffer)?

A buffer that contains descriptions of each motion transform in the acceleration structure.

var motionTransformBufferOffset: Int

The offset, in bytes, to the descripton of the first motion transform.

