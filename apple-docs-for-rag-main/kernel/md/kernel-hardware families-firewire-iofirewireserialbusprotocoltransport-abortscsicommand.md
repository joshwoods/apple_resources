

- Kernel
- Hardware Families
- FireWire
- IOFireWireSerialBusProtocolTransport
-  AbortSCSICommand 

# AbortSCSICommand

This method is intended to abort an in progress SCSI Task.

``` source
virtual SCSIServiceResponse AbortSCSICommand (
 SCSITaskIdentifier request ); 
```

## Return Value

See SCSITask.h for SCSIServiceResponse codes.

## Overview

Currently not implemented in super class. This is a stub method for adding the abort command in the near future.

## See Also

### Miscellaneous

AllocateResources

Allocate Resources.

cleanUp

cleanUp is called to tear down IOFireWireSerialBusProtocolTransport.

CoalesceSenseData

CoalesceSenseData convert a SBP-2 status block into a SPC-2 sense block.

CommandORBAccessor

accessor function for fORB.

CompleteSCSITask

This qualifies and sets appropriate data then calls CommandCompleted.

CriticalOrbSubmission

xxx\.

DeallocateResources

Deallocate Resources.

finalize

See IOService for discussion.

free

HandleProtocolServiceFeature

Handle specified feature supported by the protocol layer.

init

See IOService for discussion.

IsProtocolServiceSupported

Determine is specified feature is supported by the protocol layer.

LoginCompletion

Completion routine for login complete.

LogoutCompletion

Completion routine for logout complete.

LunResetComplete

Callback to submit Fetch Agent Reset.

SBP2LoginAccessor

accessor function for fLogin.

SendSCSICommand

Prepare and send a SCSI command to the device.

SetCommandBuffers

Method to set orb's buffers.

SetValidAutoSenseData

Set the auto sense data that was returned for a given SCSI Task.

start

StatusNotify

This is our handler for status.

UnsolicitedStatusNotify

This is our handler for unsolicited status.

