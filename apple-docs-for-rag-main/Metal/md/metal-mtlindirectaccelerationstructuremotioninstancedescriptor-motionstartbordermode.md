

- Metal
- MTLIndirectAccelerationStructureMotionInstanceDescriptor
-  motionStartBorderMode 

Instance Property

# motionStartBorderMode

The motion border mode describing what happens if Metal samples the acceleration structure before the motion start time.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var motionStartBorderMode: MTLMotionBorderMode
```

## See Also

### Specifying Motion Data

var motionStartTime: Float

The start time of the motion instance.

var motionEndTime: Float

The end time of the motion instance.

var motionEndBorderMode: MTLMotionBorderMode

The motion border mode describing what happens if Metal samples the acceleration structure after the motion end time.

var motionTransformsCount: UInt32

The number of motion transforms belonging to the motion instance.

var motionTransformsStartIndex: UInt32

The index of the first set of transforms describing one keyframe of the animation.

