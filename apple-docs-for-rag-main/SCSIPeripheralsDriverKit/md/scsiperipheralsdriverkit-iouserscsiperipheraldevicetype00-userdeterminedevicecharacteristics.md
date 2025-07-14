

- SCSIPeripheralsDriverKit
- IOUserSCSIPeripheralDeviceType00
-  UserDetermineDeviceCharacteristics 

Instance Method

# UserDetermineDeviceCharacteristics

Performs enumeration-time initializations in response to a call from the framework.

DriverKit 22.0+

``` source
kern_return_t UserDetermineDeviceCharacteristics(bool * result);
```

## Parameters 

`result`  

On return, this value is `true` if initialization succeeds; otherwise, `false`.

## Discussion

The kernel calls this user space method at enumeration time. Use this callback to perform any initializations your DriverKit extension (dext) needs to perform.

## See Also

### Managing the device

UserResetDevice

Performs a bus reset of the external drive.

