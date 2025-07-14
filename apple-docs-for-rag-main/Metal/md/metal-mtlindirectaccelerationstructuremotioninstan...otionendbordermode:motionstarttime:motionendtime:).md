

- Metal
- MTLIndirectAccelerationStructureMotionInstanceDescriptor
-  init(options:mask:intersectionFunctionTableOffset:userID:accelerationStructureID:motionTransformsStartIndex:motionTransformsCount:motionStartBorderMode:motionEndBorderMode:motionStartTime:motionEndTime:) 

Initializer

# init(options:mask:intersectionFunctionTableOffset:userID:accelerationStructureID:motionTransformsStartIndex:motionTransformsCount:motionStartBorderMode:motionEndBorderMode:motionStartTime:motionEndTime:)

Creates an indirect acceleration structure instance.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    options: MTLAccelerationStructureInstanceOptions,
    mask: UInt32,
    intersectionFunctionTableOffset: UInt32,
    userID: UInt32,
    accelerationStructureID: MTLResourceID,
    motionTransformsStartIndex: UInt32,
    motionTransformsCount: UInt32,
    motionStartBorderMode: MTLMotionBorderMode,
    motionEndBorderMode: MTLMotionBorderMode,
    motionStartTime: Float,
    motionEndTime: Float
)
```

