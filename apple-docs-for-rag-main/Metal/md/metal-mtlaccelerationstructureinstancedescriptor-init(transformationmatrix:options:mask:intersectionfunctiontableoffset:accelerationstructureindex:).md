

- Metal
- MTLAccelerationStructureInstanceDescriptor
-  init(transformationMatrix:options:mask:intersectionFunctionTableOffset:accelerationStructureIndex:) 

Initializer

# init(transformationMatrix:options:mask:intersectionFunctionTableOffset:accelerationStructureIndex:)

Creates a new acceleration structure instance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(
    transformationMatrix: MTLPackedFloat4x3,
    options: MTLAccelerationStructureInstanceOptions,
    mask: UInt32,
    intersectionFunctionTableOffset: UInt32,
    accelerationStructureIndex: UInt32
)
```

## Parameters 

`transformationMatrix`  

The transform for placing and orienting the instance in the scene.

`options`  

The options for this instance.

`mask`  

A mask to use for this instance when testing a ray against the geometry.

`intersectionFunctionTableOffset`  

An offset to apply to the intersection function table when testing a ray against this instance.

`accelerationStructureIndex`  

The index of the acceleration structure to use for this instance.

## See Also

### Creating an Instance Descriptor

init()

Creates a default acceleration structure instance.

