

- SCSIPeripheralsDriverKit
-  IOUserSCSIPeripheralDeviceType05 

Class

# IOUserSCSIPeripheralDeviceType05

A DriverKit provider object that works with type 05 devices, those that use SCSI Multimedia Commands (SMC).

DriverKit 22.0+

``` source
class IOUserSCSIPeripheralDeviceType05;
```

## Overview

Subclass this class to create a driver for multimedia devices, such as CD-ROM and DVD-ROM peripherals. In your subclass, override all pure virtual methods.

Use the functions in SCSI commands to populate Command Descriptor Blocks (CDBs) that you send to the device with UserSendCDB.

## Topics

### Managing the device

UserInitializeDeviceSupport

Performs enumeration-time initializations in response to a call from the framework.

UserResetDevice

Performs a bus reset of the external drive.

### Sending commands to the device

UserSendCDB

Sends a vendor-specific Command Descriptor Block (CDB) to the device.

SCSIType05OutParameters

Parameters for commands to send to the external SCSI device.

SCSIType05OutVersion

Constants that represent versions of the type 05 outbound interface.

SCSIType05InParameters

Parameters for responses from the external SCSI device.

SCSIType05InVersion

Constants that represent versions of the type 05 inbound interface.

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

IOUserSCSIPeripheralDeviceType00

A DriverKit provider object that works with type 00 devices, those that use SCSI Block Commands (SBC).

