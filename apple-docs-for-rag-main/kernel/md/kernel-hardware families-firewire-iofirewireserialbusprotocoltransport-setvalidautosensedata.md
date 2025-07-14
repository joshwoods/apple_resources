

- Kernel
- Hardware Families
- FireWire
- IOFireWireSerialBusProtocolTransport
-  SetValidAutoSenseData 

# SetValidAutoSenseData

Set the auto sense data that was returned for a given SCSI Task.

``` source
void SetValidAutoSenseData (
 SBP2ClientOrbData *clientData, 
 FWSBP2StatusBlock *statusBlock, 
 SCSI_Sense_Data *targetData ); 
```

## Overview

SetValidAutoSenseData is called to qualify sense data that is copied to the client via the SetAutoSenseData method. See IOSCSIProtocolServices.h for more details regarding SetAutoSenseData.

## See Also

### Miscellaneous

AbortSCSICommand

This method is intended to abort an in progress SCSI Task.

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

start

StatusNotify

This is our handler for status.

UnsolicitedStatusNotify

This is our handler for unsolicited status.

