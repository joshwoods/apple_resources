

- SCSIPeripheralsDriverKit
- IOUserSCSIPeripheralDeviceType00
-  UserResetDevice 

Instance Method

# UserResetDevice

Performs a bus reset of the external drive.

DriverKit 22.0+

``` source
kern_return_t UserResetDevice(SCSIServiceResponse * response);
```

## Parameters 

`response`  

A pointer to a SCSIServiceResponse instance. On return, the framework populates this reference with the response from the protocol driver.

## Return Value

A value that indicates the result of the bus reset. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## See Also

### Managing the device

UserDetermineDeviceCharacteristics

Performs enumeration-time initializations in response to a call from the framework.

