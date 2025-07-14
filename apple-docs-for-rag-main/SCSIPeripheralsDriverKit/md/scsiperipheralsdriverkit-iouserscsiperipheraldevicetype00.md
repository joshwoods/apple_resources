

- SCSIPeripheralsDriverKit
-  IOUserSCSIPeripheralDeviceType00 

Class

# IOUserSCSIPeripheralDeviceType00

A DriverKit provider object that works with type 00 devices, those that use SCSI Block Commands (SBC).

DriverKit 22.0+

``` source
class IOUserSCSIPeripheralDeviceType00;
```

## Overview

Subclass this class to create a driver for direct-access block devices, such as magnetic disks and solid-state drives. In your subclass, override all pure virtual methods.

Use the functions in SCSI commands to populate Command Descriptor Blocks (CDBs) that you send to the device with UserSendCDB.

## Topics

### Managing the device

UserDetermineDeviceCharacteristics

Performs enumeration-time initializations in response to a call from the framework.

UserResetDevice

Performs a bus reset of the external drive.

### Sending commands to the device

UserSendCDB

Sends a vendor-specific Command Descriptor Block (CDB) to the device.

SCSIType00OutParameters

Parameters for commands to send to the external SCSI device.

SCSIType00OutVersion

Constants that represent versions of the type 00 outbound interface.

SCSIType00InParameters

Parameters for responses from the external SCSI device.

SCSIType00InVersion

Constants that represent versions of the type 00 inbound interface.

### Suspending and resuming services

UserSuspendServices

Suspends services and allows the dext to communicate with the external drive.

UserResumeServices

Resumes normal services after a suspension.

### Providing device metadata

UserReportMediumBlockSize

Provides a report on the external device’s block size.

## Relationships

### Inherits From

- IOService

## See Also

### Driver interfaces

IOUserSCSIPeripheralDeviceType05

A DriverKit provider object that works with type 05 devices, those that use SCSI Multimedia Commands (SMC).

