

- SCSIControllerDriverKit
- SCSIUserParallelTask
-  fControllerTaskIdentifier 

Instance Property

# fControllerTaskIdentifier

A unique identifier for a task.

DriverKit

``` source
uint64_t fControllerTaskIdentifier;
```

## See Also

### Task Properties

version

The version of the parallel task structure currently in use.

SCSIUserParallelTaskVersion

Constants that represent versions of the user parallel task structure.

fTargetID

An identifier that represents a SCSI target device.

fSCSIParallelFeatureRequest

An array of features of the SCSI parallel interface to negotiate.

SCSIParallelFeatureRequest

An enumeration of feature negotiation behaviors.

fSCSIParallelFeatureRequestCount

The number of features to negotiate.

fRequestedTransferCount

The requested data transfer count for the request’s data.

fBufferIOVMAddr

The start address of the generated physical segment of the data buffer.

fTaskAttribute

The SCSI task attribute of the task.

fTaskTagIdentifier

A 64-bit number that represents a unique task identifier.

fLogicalUnitBytes

The request’s logical unit bytes.

fCommandDescriptorBlock

The task’s SCSI command descriptor block.

fCommandSize

The size of the SCSI command descriptor block in bytes.

fTransferDirection

The direction of data transfer for this task.

reserved

An unused field reserved for future use.

