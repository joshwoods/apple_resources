

- SCSIPeripheralsDriverKit
-  SCSIDeviceInParameters 

Structure

# SCSIDeviceInParameters

A structure that contains properties from an inbound response from a SCSI device.

DriverKit 22.0+

``` source
typedef struct SCSIDeviceInParameters { ... } SCSIDeviceInParameters;
```

## Topics

### Accessing response properties

fCompletionStatus

The status of the task at completion of the call, such as good, busy, or timeout.

fServiceResponse

The response from the service, such as complete, in process, or rejected.

fRealizedByteCountOfTransfer

The byte count of the tranferred data.

fSenseDataValid

A Boolean value that indicates whether the sense data that the kernel provides is valid.

### Infrequently Used Functionality

reserved

An unused field reserved for future use.

## Relationships

### Inherited By

- SCSIType00InParameters
- SCSIType05InParameters
- SCSIType07InParameters

## See Also

### Supporting types

SCSIDeviceOutParameters

A structure that contains parameters for an outbound request to a SCSI device.

