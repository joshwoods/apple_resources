

- SCSIPeripheralsDriverKit
- SCSIDeviceOutParameters
-  fBufferDirection 

Instance Property

# fBufferDirection

The direction for the buffer to send or receive data.

DriverKit 22.0+

``` source
uint8_t fBufferDirection;
```

## Discussion

Use the following `DriverKit/IOMemoryDescriptor.h` direction values to populate this field:

- kIOMemoryDirectionNone

- kIOMemoryDirectionIn

- kIOMemoryDirectionOut

- kIOMemoryDirectionOutIn

- kIOMemoryDirectionInOut

- kIOMemoryDisableCopyOnWrite

## See Also

### Setting command parameters

fLogicalUnitNumber

The SCSI logical unit number of the device that receives the command.

fTimeoutDuration

A timeout for the command, in milliseconds.

fCommandDescriptorBlock

A 16-byte opcode to fill out the Command Descriptor Block (CDB).

fRequestedByteCountOfTransfer

The size of the data to transfer.

fDataTransferDirection

The direction for the caller to send data to or receive data from the device.

fSenseLengthRequested

The length of sense data to read, in bytes.

fDataBufferAddr

The virtual address of the buffer the dext creates to transfer data.

fSenseBufferAddr

The virtual address of the buffer that the dext creates to transfer sense data.

