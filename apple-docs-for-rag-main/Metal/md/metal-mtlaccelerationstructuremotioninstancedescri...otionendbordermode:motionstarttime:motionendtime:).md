

- Metal
- MTLAccelerationStructureMotionInstanceDescriptor
-  init(options:mask:intersectionFunctionTableOffset:accelerationStructureIndex:userID:motionTransformsStartIndex:motionTransformsCount:motionStartBorderMode:motionEndBorderMode:motionStartTime:motionEndTime:) 

Initializer

# init(options:mask:intersectionFunctionTableOffset:accelerationStructureIndex:userID:motionTransformsStartIndex:motionTransformsCount:motionStartBorderMode:motionEndBorderMode:motionStartTime:motionEndTime:)

Creates a new acceleration structure instance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    options: MTLAccelerationStructureInstanceOptions,
    mask: UInt32,
    intersectionFunctionTableOffset: UInt32,
    accelerationStructureIndex: UInt32,
    userID: UInt32,
    motionTransformsStartIndex: UInt32,
    motionTransformsCount: UInt32,
    motionStartBorderMode: MTLMotionBorderMode,
    motionEndBorderMode: MTLMotionBorderMode,
    motionStartTime: Float,
    motionEndTime: Float
)
```

## Parameters 

`options`  

An option set for new acceleration-structure motion-instances.

`mask`  

A mask for testing ray-tracing rays in a scene’s geometry for new acceleration-structure motion-instances.

`intersectionFunctionTableOffset`  

An offset into the intersection-function table for ray tracing.

`accelerationStructureIndex`  

The index of an acceleration structure that applies to new acceleration-structure motion-instances.

`userID`  

An unique identifier for an acceleration-structure motion-instance.

`motionTransformsStartIndex`  

An index of the motion data that represents the first key-frame’s motion data.

`motionTransformsCount`  

The number of motion data key-frames that begin at motionTransformsStartIndex.

`motionStartBorderMode`  

A behavior that configures how an acceleration-structure motion-instance handles timestamps before motionStartTime.

`motionEndBorderMode`  

A behavior that configures how an acceleration-structure motion-instance handles timestamps after motionEndTime.

`motionStartTime`  

A starting time for the range of motion that the key-frame data (see motionTransformsStartIndex and motionTransformsCount) represent.

`motionEndTime`  

An ending time for the range of motion that the key-frame data (see motionTransformsStartIndex and motionTransformsCount) represent.

## See Also

### Creating an Instance Descriptor

init()

Creates a default acceleration structure instance.

