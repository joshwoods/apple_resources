

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserSetTargetProperties 

Instance Method

# UserSetTargetProperties

Sets properties on the target.

DriverKit

``` source
kern_return_t UserSetTargetProperties(SCSIDeviceIdentifier targetID, OSDictionary * properties);
```

## Parameters 

`targetID`  

The ID of the target with the properties you want to set.

`properties`  

A dictionary containing key-value pairs of properties to set.

## Return Value

A value that indicates the result of setting the target’s properties. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

Your driver extension calls this method to set the specified target’s properties. The `properties` directory can contain the following keys:

- kIOPropertySASAddressKey

- kIOPropertyFibreChannelNodeWorldWideNameKey

- kIOPropertyFibreChannelPortWorldWideNameKey

- kIOPropertyFibreChannelAddressIdentifierKey

- kIOPropertyFibreChannelALPAKey.

The value of each property should be a pointer to a valid OSString object that represents the value for the property. The value must be of the proper type and size for the specified key.

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

UserRemoveTargetProperties

Removes properties from a target.

