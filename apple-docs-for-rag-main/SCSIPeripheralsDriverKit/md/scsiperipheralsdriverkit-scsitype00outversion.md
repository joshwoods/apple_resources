

- SCSIPeripheralsDriverKit
-  SCSIType00OutVersion 

Enumeration

# SCSIType00OutVersion

Constants that represent versions of the type 00 outbound interface.

DriverKit 22.0+

``` source
typedef enum SCSIType00OutVersion : unsigned int { ... } SCSIType00OutVersion;
```

## Topics

### Versions

kScsiType00OutCurrentVersion1

Version 1 of the type 00 outbound interface.

## See Also

### Sending commands to the device

UserSendCDB

Sends a vendor-specific Command Descriptor Block (CDB) to the device.

SCSIType00OutParameters

Parameters for commands to send to the external SCSI device.

SCSIType00InParameters

Parameters for responses from the external SCSI device.

SCSIType00InVersion

Constants that represent versions of the type 00 inbound interface.

