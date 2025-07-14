

- SCSIPeripheralsDriverKit
- IOUserSCSIPeripheralDeviceType05
-  UserInitializeDeviceSupport 

Instance Method

# UserInitializeDeviceSupport

Performs enumeration-time initializations in response to a call from the framework.

DriverKit 22.0+

``` source
kern_return_t UserInitializeDeviceSupport(bool * result);
```

## Discussion

The kernel calls this user space method at enumeration time. Use this callback to perform any initializations your DriverKit extension (dext) needs to perform.

## See Also

### Managing the device

UserResetDevice

Performs a bus reset of the external drive.

