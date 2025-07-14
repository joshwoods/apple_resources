

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserCreateTargetForID 

Instance Method

# UserCreateTargetForID

Creates the specified target.

DriverKit

``` source
kern_return_t UserCreateTargetForID(SCSIDeviceIdentifier targetID, OSDictionary * targetDict);
```

## Parameters 

`targetID`  

The ID of the target to create.

`targetDict`  

An OSDictionary containing all of the target properties.

## Return Value

A value that indicates the result of target creation. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

Your driver extension class calls this method to create a new target for the `targetID`. The framework creates the new target before the call returns.

As part of the UserCreateTargetForID call, the kernel calls several APIs like UserInitializeTargetForID which run on the default dispatch queue of the dext. Synchronously calling UserCreateTargetForID from the default dispatch queue blocks the default dispatch queue until UserCreateTargetForID finishes. Subsequent calls from the kernel like UserInitializeTargetForID won’t have a chance to run on the default queue, leading to a deadlock.

You can avoid this problem by calling UserCreateTargetForID from an asynchronous handler function. Start by creating an async handler function for your custom dext class in its `iig` file, as shown below:

```
virtual void AsyncEventHandler ( OSAction *  action TARGET,                                 uint32_t    targetID ) = 0;

virtual void AsyncCreateTargetForID ( OSAction *  action,
                                    uint32_t    targetID )
                                    TYPE ( ExampleSCSIDext::AsyncEventHandler ) QUEUENAME ( AuxiliaryQueue );
```

This handler function can then call UserCreateTargetForID:

```
void
IMPL ( MyCustomService, AsyncCreateTargetForID )
{
     kern_return_t ret;
     …
     ret = UserCreateTargetForID (targetID, NULL);
     …
}
```

Then you can call this handler in UserStartController:

```
kern_return_t
IMPL ( MyCustomService, UserStartController )
{
    …
    ret = CreateActionAsyncCreateTargetForID ( sizeof ( void * ), &ivars->fAsyncEventHandler );
    assert ( kIOReturnSuccess == ret );

    AsyncEventHandler ( ivars->fAsyncEventHandler, targetID );
    …
}
```

This implementation ensures UserStartController calls the event handler asynchronously, which frees up the default dispatch queue for subsequent calls.

## See Also

### Managing Targets

UserInitializeTargetForID

Initializes a target device in response to a call from the framework.

UserDestroyTargetForID

Destroys the specified target.

UserTargetPresentForID

Checks if a specific target is present.

UserSetTargetProperties

Sets properties on the target.

UserRemoveTargetProperties

Removes properties from a target.

