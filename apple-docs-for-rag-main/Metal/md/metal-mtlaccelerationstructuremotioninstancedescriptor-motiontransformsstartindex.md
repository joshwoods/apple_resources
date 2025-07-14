

- Metal
- MTLAccelerationStructureMotionInstanceDescriptor
-  motionTransformsStartIndex 

Instance Property

# motionTransformsStartIndex

The index for the instance’s first keyframe motion data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var motionTransformsStartIndex: UInt32
```

## Discussion

The index points to an entry in the MTLInstanceAccelerationStructureDescriptor’s transform data, stored in its motionTransformBuffer property.

## See Also

### Specifying Motion Data

var motionStartTime: Float

The start time for the range of motion described by the keyframe data.

var motionEndTime: Float

The end time for the range of motion described by the keyframe data.

var motionStartBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps before the start time.

var motionEndBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps after the end time.

var motionTransformsCount: UInt32

The number of keyframes for this instance.

