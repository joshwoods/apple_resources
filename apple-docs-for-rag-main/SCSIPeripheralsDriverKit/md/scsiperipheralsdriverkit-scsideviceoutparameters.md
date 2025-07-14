

- SCSIPeripheralsDriverKit
-  SCSIDeviceOutParameters 

Structure

# SCSIDeviceOutParameters

A structure that contains parameters for an outbound request to a SCSI device.

DriverKit 22.0+

``` source
typedef struct SCSIDeviceOutParameters { ... } SCSIDeviceOutParameters;
```

## Topics

### Setting command parameters

fLogicalUnitNumber

The SCSI logical unit number of the device that receives the command.

fTimeoutDuration

A timeout for the command, in milliseconds.

fCommandDescriptorBlock

A 16-byte opcode to fill out the Command Descriptor Block (CDB).

fRequestedByteCountOfTransfer

The size of the data to transfer.

fBufferDirection

The direction for the buffer to send or receive data.

fDataTransferDirection

The direction for the caller to send data to or receive data from the device.

fSenseLengthRequested

The length of sense data to read, in bytes.

fDataBufferAddr

The virtual address of the buffer the dext creates to transfer data.

fSenseBufferAddr

The virtual address of the buffer that the dext creates to transfer sense data.

### Infrequently Used Functionality

reserved

An unused field reserved for future use.

## Relationships

### Inherited By

- SCSIType00OutParameters
- SCSIType05OutParameters
- SCSIType07OutParameters

## See Also

### Supporting types

SCSIDeviceInParameters

A structure that contains properties from an inbound response from a SCSI device.

