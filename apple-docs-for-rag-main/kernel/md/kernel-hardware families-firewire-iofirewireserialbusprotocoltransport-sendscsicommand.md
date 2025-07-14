

- Kernel
- Hardware Families
- FireWire
- IOFireWireSerialBusProtocolTransport
-  SendSCSICommand 

# SendSCSICommand

Prepare and send a SCSI command to the device.

``` source
virtual bool SendSCSICommand (
 SCSITaskIdentifier request, 
 SCSIServiceResponse *serviceResponse, 
 SCSITaskStatus *taskStatus ); 
```

## Return Value

If the command was sent to the device and is pending completion, the subclass should return true and return back the kSCSIServiceResponse_Request_In_Process response. If the command completes immediately with an error, the subclass will return true and return back the appropriate status. If the subclass is currently processing all the commands it can, the subclass will return false and the command will be resent next time CommandCompleted is called.

## Overview

The incoming SCSITaskIdentifier gets turned into a IOFireWireSBP2ORB and is submitted to the SBP2 layer. See IOSCSIProtocolServices.h for more details regarding SendSCSICommand. Also see IOFireWireSBP2Lib.h for details regarding the IOFireWireSBP2ORB structure and the submitORB method.

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

SetCommandBuffers

Method to set orb's buffers.

SetValidAutoSenseData

Set the auto sense data that was returned for a given SCSI Task.

start

StatusNotify

This is our handler for status.

UnsolicitedStatusNotify

This is our handler for unsolicited status.

