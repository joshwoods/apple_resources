

- Metal
- MTLPrimitiveAccelerationStructureDescriptor
-  motionKeyframeCount 

Instance Property

# motionKeyframeCount

The number of keyframes in the geometry data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var motionKeyframeCount: Int { get set }
```

## Discussion

The default value is `1`. If the value is greater than `1`, all geometry descriptors that you attach to this descriptor must be motion descriptors, and each must have exactly that many MTLMotionKeyframeData objects.

## See Also

### Related Documentation

var geometryDescriptors: [MTLAccelerationStructureGeometryDescriptor]?

An array that contains the individual pieces of geometry that compose the acceleration structure.

### Specifying Motion Behavior

var motionStartTime: Float

The start time for the range of motion that the keyframe data describes.

var motionEndTime: Float

The end time for the range of motion that the keyframe data describes.

var motionStartBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps before the start time.

var motionEndBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps after the end time.

enum MTLMotionBorderMode

Options for specifying how the acceleration structure handles timestamps that are outside the specified range.

