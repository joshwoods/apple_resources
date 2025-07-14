

- Kernel
- Hardware Families
- FireWire
- IOFireWireSerialBusProtocolTransport
-  finalize 

# finalize

See IOService for discussion.

``` source
virtual bool finalize (
 IOOptionBits options ); 
```

## Return Value

Returns true.

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

