

- SCSIPeripheralsDriverKit
- IOUserSCSIPeripheralDeviceType00
-  UserSendCDB 

Instance Method

# UserSendCDB

Sends a vendor-specific Command Descriptor Block (CDB) to the device.

DriverKit 22.0+

``` source
kern_return_t UserSendCDB(SCSIType00OutParameters command, SCSIType00InParameters * response);
```

## Parameters 

`command`  

A SCSIType00OutParameters instance that contains the request information.

`response`  

A pointer to a SCSIType00InParameters instance. On return, the framework fills this object with the response data.

## Return Value

A value that indicates the result of sending the CDB. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

Call this method to deliver vendor-specific 16-byte commands to the external drive that this dext matches.

## See Also

### Sending commands to the device

SCSIType00OutParameters

Parameters for commands to send to the external SCSI device.

SCSIType00OutVersion

Constants that represent versions of the type 00 outbound interface.

SCSIType00InParameters

Parameters for responses from the external SCSI device.

SCSIType00InVersion

Constants that represent versions of the type 00 inbound interface.

