

- SCSIPeripheralsDriverKit
-  SCSIType00InVersion 

Enumeration

# SCSIType00InVersion

Constants that represent versions of the type 00 inbound interface.

DriverKit 22.0+

``` source
typedef enum SCSIType00InVersion : unsigned int { ... } SCSIType00InVersion;
```

## Topics

### Versions

kScsiType00InCurrentVersion1

Version 1 of the type 00 inbound interface.

## See Also

### Sending commands to the device

UserSendCDB

Sends a vendor-specific Command Descriptor Block (CDB) to the device.

SCSIType00OutParameters

Parameters for commands to send to the external SCSI device.

SCSIType00OutVersion

Constants that represent versions of the type 00 outbound interface.

SCSIType00InParameters

Parameters for responses from the external SCSI device.

