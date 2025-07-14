

- Metal
- MTLAccelerationStructureMotionInstanceDescriptor
-  motionEndTime 

Instance Property

# motionEndTime

The end time for the range of motion described by the keyframe data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var motionEndTime: Float
```

## Discussion

The default value is `1.0f`.

## See Also

### Specifying Motion Data

var motionStartTime: Float

The start time for the range of motion described by the keyframe data.

var motionStartBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps before the start time.

var motionEndBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps after the end time.

var motionTransformsStartIndex: UInt32

The index for the instance’s first keyframe motion data.

var motionTransformsCount: UInt32

The number of keyframes for this instance.

