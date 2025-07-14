

- SCSIPeripheralsDriverKit
- SCSIDeviceOutParameters
-  fCommandDescriptorBlock 

Instance Property

# fCommandDescriptorBlock

A 16-byte opcode to fill out the Command Descriptor Block (CDB).

DriverKit 22.0+

``` source
SCSICommandDescriptorBlock fCommandDescriptorBlock;
```

## Discussion

Populate this member of the parameters structure with the functions listed in the following sections:

- Creating common SCSI commands

- Creating Self-Monitoring, Analysis and Reporting Technology (SMART) Commands

- Creating arbitrary SCSI commands

## See Also

### Setting command parameters

fLogicalUnitNumber

The SCSI logical unit number of the device that receives the command.

fTimeoutDuration

A timeout for the command, in milliseconds.

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

