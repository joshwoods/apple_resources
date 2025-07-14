

- SCSIPeripheralsDriverKit
-  SCSIType05OutVersion 

Enumeration

# SCSIType05OutVersion

Constants that represent versions of the type 05 outbound interface.

DriverKit 22.0+

``` source
typedef enum SCSIType05OutVersion : unsigned int { ... } SCSIType05OutVersion;
```

## Topics

### Versions

kScsiType05OutCurrentVersion1

Version 1 of the type 05 outbound interface.

## See Also

### Sending commands to the device

UserSendCDB

Sends a vendor-specific Command Descriptor Block (CDB) to the device.

SCSIType05OutParameters

Parameters for commands to send to the external SCSI device.

SCSIType05InParameters

Parameters for responses from the external SCSI device.

SCSIType05InVersion

Constants that represent versions of the type 05 inbound interface.

