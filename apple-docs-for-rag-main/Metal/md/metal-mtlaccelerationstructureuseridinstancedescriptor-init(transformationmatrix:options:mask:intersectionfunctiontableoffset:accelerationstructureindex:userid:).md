

- Metal
- MTLAccelerationStructureUserIDInstanceDescriptor
-  init(transformationMatrix:options:mask:intersectionFunctionTableOffset:accelerationStructureIndex:userID:) 

Initializer

# init(transformationMatrix:options:mask:intersectionFunctionTableOffset:accelerationStructureIndex:userID:)

Creates a new acceleration structure instance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    transformationMatrix: MTLPackedFloat4x3,
    options: MTLAccelerationStructureInstanceOptions,
    mask: UInt32,
    intersectionFunctionTableOffset: UInt32,
    accelerationStructureIndex: UInt32,
    userID: UInt32
)
```

## Parameters 

`transformationMatrix`  

The transform for placing and orienting the instance in the scene.

`options`  

The options for the instance.

`mask`  

A mask to use for the instance when testing a ray against the geometry.

`intersectionFunctionTableOffset`  

An offset to apply to the intersection function table when testing a ray against the instance.

`accelerationStructureIndex`  

The index of the acceleration structure to use for the instance.

`userID`  

The user identifier for the instance.

## See Also

### Creating an Instance Descriptor

init()

Creates a default acceleration structure instance.

