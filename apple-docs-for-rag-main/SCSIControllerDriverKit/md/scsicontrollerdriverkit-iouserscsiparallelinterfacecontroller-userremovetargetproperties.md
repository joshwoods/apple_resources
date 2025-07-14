

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserRemoveTargetProperties 

Instance Method

# UserRemoveTargetProperties

Removes properties from a target.

DriverKit

``` source
kern_return_t UserRemoveTargetProperties(SCSIDeviceIdentifier targetID, OSArray * properties);
```

## Parameters 

`targetID`  

The ID of the target with the properties you want to remove.

`properties`  

An array containing keys of the properties to remove.

## Return Value

A value that indicates the result of setting the target’s specified properties. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

Your driver extension calls this method to remove the specified properties from the target.

## See Also

### Managing Targets

UserInitializeTargetForID

Initializes a target device in response to a call from the framework.

UserCreateTargetForID

Creates the specified target.

UserDestroyTargetForID

Destroys the specified target.

UserTargetPresentForID

Checks if a specific target is present.

UserSetTargetProperties

Sets properties on the target.

