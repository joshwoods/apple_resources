

- Metal
-  MTLMotionBorderMode 

Enumeration

# MTLMotionBorderMode

Options for specifying how the acceleration structure handles timestamps that are outside the specified range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
enum MTLMotionBorderMode
```

## Overview

The motionStartBorderMode and motionEndBorderMode properties use this type to describe the behavior for a motion-based object when a timestamp is outside the specified range.

## Topics

### Specifying Motion Modes

case clamp

A mode that specifies treating times outside the specified endpoint as if they were at the endpoint.

case vanish

A mode that specifies that times outside the specified endpoint need to prevent any ray-intersections with the primitive.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying Motion Behavior

var motionKeyframeCount: Int

The number of keyframes in the geometry data.

var motionStartTime: Float

The start time for the range of motion that the keyframe data describes.

var motionEndTime: Float

The end time for the range of motion that the keyframe data describes.

var motionStartBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps before the start time.

var motionEndBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps after the end time.

