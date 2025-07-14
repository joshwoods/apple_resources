

- Metal
- MTLPrimitiveAccelerationStructureDescriptor
-  motionStartBorderMode 

Instance Property

# motionStartBorderMode

The mode to use when handling timestamps before the start time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var motionStartBorderMode: MTLMotionBorderMode { get set }
```

## Discussion

The default value is MTLMotionBorderMode.clamp.

## See Also

### Specifying Motion Behavior

var motionKeyframeCount: Int

The number of keyframes in the geometry data.

var motionStartTime: Float

The start time for the range of motion that the keyframe data describes.

var motionEndTime: Float

The end time for the range of motion that the keyframe data describes.

var motionEndBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps after the end time.

enum MTLMotionBorderMode

Options for specifying how the acceleration structure handles timestamps that are outside the specified range.

