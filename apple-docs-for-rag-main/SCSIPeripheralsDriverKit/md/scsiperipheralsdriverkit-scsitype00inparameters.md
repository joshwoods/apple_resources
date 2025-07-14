

- SCSIPeripheralsDriverKit
-  SCSIType00InParameters 

Structure

# SCSIType00InParameters

Parameters for responses from the external SCSI device.

DriverKit 22.0+

``` source
struct SCSIType00InParameters;
```

## Discussion

This type contains all the fields from SCSIDeviceInParameters, typed for use only with IOUserSCSIPeripheralDeviceType00 devices.

## Relationships

### Inherits From

- SCSIDeviceInParameters

## See Also

### Sending commands to the device

UserSendCDB

Sends a vendor-specific Command Descriptor Block (CDB) to the device.

SCSIType00OutParameters

Parameters for commands to send to the external SCSI device.

SCSIType00OutVersion

Constants that represent versions of the type 00 outbound interface.

SCSIType00InVersion

Constants that represent versions of the type 00 inbound interface.

