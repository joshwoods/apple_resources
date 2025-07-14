

- Kernel
- Hardware Families
- FireWire
- IOFireWireSerialBusProtocolTransport
-  CoalesceSenseData 

# CoalesceSenseData

CoalesceSenseData convert a SBP-2 status block into a SPC-2 sense block.

``` source
SCSITaskStatus CoalesceSenseData (
 FWSBP2StatusBlock *sourceData, 
 UInt8 quadletCount, 
 SCSI_Sense_Data *targetData ); 
```

## Overview

CoalesceSenseData pulls the appropriate bits out of the SBP2 sense block as defined in SBP-2 Annex B section B.2 and dynamically builds a sense data block as defined in SPC-2 section 7.23.2.

## See Also

### Miscellaneous

AbortSCSICommand

This method is intended to abort an in progress SCSI Task.

AllocateResources

Allocate Resources.

cleanUp

cleanUp is called to tear down IOFireWireSerialBusProtocolTransport.

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

