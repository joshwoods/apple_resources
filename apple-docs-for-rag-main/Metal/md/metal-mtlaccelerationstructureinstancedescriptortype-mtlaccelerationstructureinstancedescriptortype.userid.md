

- Metal
- MTLAccelerationStructureInstanceDescriptorType
-  MTLAccelerationStructureInstanceDescriptorType.userID 

Case

# MTLAccelerationStructureInstanceDescriptorType.userID

An option specifying that the instance contains a user identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
case userID
```

## Discussion

This instance type corresponds to the MTLAccelerationStructureUserIDInstanceDescriptor structure memory layout.

## See Also

### Specifying the Instance Descriptor Type

case `default`

An option specifying that the instance uses the default characteristics.

case motion

An option specifying that the instance contains motion data.

case indirect

An option that enables using an instance descriptor memory layout that the GPU can populate.

case indirectMotion

An option specifying that the instance contains motion data, and enables using an instance descriptor memory layout that the GPU can populate.

