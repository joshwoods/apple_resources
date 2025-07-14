

- SCSIPeripheralsDriverKit
-  SCSIType00OutParameters 

Structure

# SCSIType00OutParameters

Parameters for commands to send to the external SCSI device.

DriverKit 22.0+

``` source
struct SCSIType00OutParameters;
```

## Discussion

This type contains all the fields from SCSIDeviceOutParameters, typed for use only with IOUserSCSIPeripheralDeviceType00 devices.

## Relationships

### Inherits From

- SCSIDeviceOutParameters

## See Also

### Sending commands to the device

UserSendCDB

Sends a vendor-specific Command Descriptor Block (CDB) to the device.

SCSIType00OutVersion

Constants that represent versions of the type 00 outbound interface.

SCSIType00InParameters

Parameters for responses from the external SCSI device.

SCSIType00InVersion

Constants that represent versions of the type 00 inbound interface.

