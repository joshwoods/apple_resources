

- Metal
- MTLPrimitiveAccelerationStructureDescriptor
-  motionStartTime 

Instance Property

# motionStartTime

The start time for the range of motion that the keyframe data describes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var motionStartTime: Float { get set }
```

## Discussion

The default value is `0.0f`.

## See Also

### Specifying Motion Behavior

var motionKeyframeCount: Int

The number of keyframes in the geometry data.

var motionEndTime: Float

The end time for the range of motion that the keyframe data describes.

var motionStartBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps before the start time.

var motionEndBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps after the end time.

enum MTLMotionBorderMode

Options for specifying how the acceleration structure handles timestamps that are outside the specified range.

