

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserInitializeTargetForID 

Instance Method

# UserInitializeTargetForID

Initializes a target device in response to a call from the framework.

DriverKit

``` source
kern_return_t UserInitializeTargetForID(SCSITargetIdentifier targetID);
```

## Parameters 

`targetID`  

The target to initialize.

## Return Value

A value that indicates the result of initialization. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

The host bus adapter (HBA) can use this method to probe the target or do anything else necessary before IOKit registers the device object for matching.

## See Also

### Managing Targets

UserCreateTargetForID

Creates the specified target.

UserDestroyTargetForID

Destroys the specified target.

UserTargetPresentForID

Checks if a specific target is present.

UserSetTargetProperties

Sets properties on the target.

UserRemoveTargetProperties

Removes properties from a target.

