

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserDestroyTargetForID 

Instance Method

# UserDestroyTargetForID

Destroys the specified target.

DriverKit

``` source
kern_return_t UserDestroyTargetForID(SCSITargetIdentifier targetID);
```

## Parameters 

`targetID`  

The ID of the target to destroy.

## Return Value

A value that indicates the result of target removal. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

Your driver extension calls this method to remove the target with the specified `targetID`.

## See Also

### Managing Targets

UserInitializeTargetForID

Initializes a target device in response to a call from the framework.

UserCreateTargetForID

Creates the specified target.

UserTargetPresentForID

Checks if a specific target is present.

UserSetTargetProperties

Sets properties on the target.

UserRemoveTargetProperties

Removes properties from a target.

