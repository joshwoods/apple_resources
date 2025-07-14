

- Metal
- MTLAccelerationStructureInstanceDescriptorType
-  MTLAccelerationStructureInstanceDescriptorType.indirectMotion 

Case

# MTLAccelerationStructureInstanceDescriptorType.indirectMotion

An option specifying that the instance contains motion data, and enables using an instance descriptor memory layout that the GPU can populate.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
case indirectMotion
```

## Discussion

This instance type corresponds to the MTLIndirectAccelerationStructureMotionInstanceDescriptor memory layout.

## See Also

### Specifying the Instance Descriptor Type

case `default`

An option specifying that the instance uses the default characteristics.

case userID

An option specifying that the instance contains a user identifier.

case motion

An option specifying that the instance contains motion data.

case indirect

An option that enables using an instance descriptor memory layout that the GPU can populate.

