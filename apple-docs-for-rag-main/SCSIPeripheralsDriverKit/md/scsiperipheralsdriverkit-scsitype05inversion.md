

- SCSIPeripheralsDriverKit
-  SCSIType05InVersion 

Enumeration

# SCSIType05InVersion

Constants that represent versions of the type 05 inbound interface.

DriverKit 22.0+

``` source
typedef enum SCSIType05InVersion : unsigned int { ... } SCSIType05InVersion;
```

## Topics

### Versions

kScsiType05InCurrentVersion1

Version 1 of the type 05 inbound interface.

## See Also

### Sending commands to the device

UserSendCDB

Sends a vendor-specific Command Descriptor Block (CDB) to the device.

SCSIType05OutParameters

Parameters for commands to send to the external SCSI device.

SCSIType05OutVersion

Constants that represent versions of the type 05 outbound interface.

SCSIType05InParameters

Parameters for responses from the external SCSI device.

