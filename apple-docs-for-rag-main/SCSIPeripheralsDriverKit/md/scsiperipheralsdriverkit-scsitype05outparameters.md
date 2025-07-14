

- SCSIPeripheralsDriverKit
-  SCSIType05OutParameters 

Structure

# SCSIType05OutParameters

Parameters for commands to send to the external SCSI device.

DriverKit 22.0+

``` source
struct SCSIType05OutParameters;
```

## Discussion

This type contains all the fields from SCSIDeviceOutParameters, typed for use only with IOUserSCSIPeripheralDeviceType05 devices.

## Relationships

### Inherits From

- SCSIDeviceOutParameters

## See Also

### Sending commands to the device

UserSendCDB

Sends a vendor-specific Command Descriptor Block (CDB) to the device.

SCSIType05OutVersion

Constants that represent versions of the type 05 outbound interface.

SCSIType05InParameters

Parameters for responses from the external SCSI device.

SCSIType05InVersion

Constants that represent versions of the type 05 inbound interface.

