

- SCSIControllerDriverKit
-  SCSIParallelFeatureResult 

Enumeration

# SCSIParallelFeatureResult

An enumeration of feature negotiation results.

DriverKit

``` source
typedef enum SCSIParallelFeatureResult : unsigned int { ... } SCSIParallelFeatureResult;
```

## Topics

### Results

kSCSIParallelFeature_NegotitiationSuccess

A result that indicates the controller negotiated successfully.

kSCSIParallelFeature_NegotitiationCleared

A result that indicates the controller cleared negotiation.

kSCSIParallelFeature_NegotitiationUnchanged

A result that indicates the controller negotiation state didn’t change.

## See Also

### Response Properties

version

The version of the parallel response structure currently in use.

SCSIUserParallelResponseVersion

Constants that represent versions of the user parallel task structure.

fTargetID

An identifier that represents a SCSI target device.

fSCSIParallelFeatureResult

An array of features the system successfully negotiated with the SCSI parallel interface.

fSCSIParallelFeatureRequestResultCount

The number of negotiated features.

fControllerTaskIdentifier

A unique identifier for a task.

fCompletionStatus

The status of the task after the host bus adapter (HBA) completes processing.

fServiceResponse

Attributes of the task service response.

fBytesTransferred

The total number of bytes the system transferred as part of the I/O with the interface.

fSenseBuffer

The SCSI sense data buffer.

fSenseLength

The length of the sense buffer, if any.

kMaxSenseBufferSize

The maximum size of the SCSI sense data buffer in a response.

reserved

An unused field reserved for future use.

