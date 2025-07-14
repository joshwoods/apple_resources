

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserTargetPresentForID 

Instance Method

# UserTargetPresentForID

Checks if a specific target is present.

DriverKit

``` source
kern_return_t UserTargetPresentForID(SCSIDeviceIdentifier targetID, bool * result);
```

## Parameters 

`targetID`  

The ID of the target to check.

`result`  

A pointer to a Boolean value that the framework sets to `true` if the target is present and `false` otherwise.

## Return Value

A value that indicates the result of checking for the target’s existence. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

Your driver extension can call this method to determine if a target ID is actually present.

## See Also

### Managing Targets

UserInitializeTargetForID

Initializes a target device in response to a call from the framework.

UserCreateTargetForID

Creates the specified target.

UserDestroyTargetForID

Destroys the specified target.

UserSetTargetProperties

Sets properties on the target.

UserRemoveTargetProperties

Removes properties from a target.

