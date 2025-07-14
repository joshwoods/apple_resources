

- Metal
- MTLAccelerationStructureInstanceDescriptorType
-  MTLAccelerationStructureInstanceDescriptorType.motion 

Case

# MTLAccelerationStructureInstanceDescriptorType.motion

An option specifying that the instance contains motion data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
case motion
```

## Discussion

This instance type corresponds to the MTLAccelerationStructureMotionInstanceDescriptor structure memory layout.

## See Also

### Specifying the Instance Descriptor Type

case `default`

An option specifying that the instance uses the default characteristics.

case userID

An option specifying that the instance contains a user identifier.

case indirect

An option that enables using an instance descriptor memory layout that the GPU can populate.

case indirectMotion

An option specifying that the instance contains motion data, and enables using an instance descriptor memory layout that the GPU can populate.

