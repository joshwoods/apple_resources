

- Kernel
- Hardware Families
- FireWire
-  IOFireWireSerialBusProtocolTransport 

Class

# IOFireWireSerialBusProtocolTransport

SCSI Protocol Driver Family for FireWire SBP2 Devices.

macOS 10.0+

``` source
class IOFireWireSerialBusProtocolTransport : IOSCSIProtocolServices
```

## Overview

IOFireWireSerialBusProtocolTransport contains all the bus specific support for FireWire SBP2 compliant devices. To add vendor specific features or workarounds you will sub-class the appropriate methods of this family.

## Topics

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

SetValidAutoSenseData

Set the auto sense data that was returned for a given SCSI Task.

start

StatusNotify

This is our handler for status.

UnsolicitedStatusNotify

This is our handler for unsolicited status.

### DataTypes

SBP2ClientOrbData

### Instance Methods

- AbortSCSICommand

- AllocateResources

- CoalesceSenseData

- CommandORBAccessor

- CompleteSCSITask

- ConnectToDevice

- CriticalOrbSubmission

- DeallocateResources

- DisconnectFromDevice

- FetchAgentResetComplete

- HandleProtocolServiceFeature

- IsDeviceCPUInDiskMode

- IsProtocolServiceSupported

- LoginCompletion

- LogoutCompletion

- LunResetComplete

- SBP2LoginAccessor

- SendSCSICommand

- SetCommandBuffers

- SetValidAutoSenseData

- StatusNotify

- UnsolicitedStatusNotify

- cleanUp

- finalize

- free

- getMetaClass

- init

- login

- loginLost

- loginResumed

- loginSuspended

- message

- start

- submitLogin

- submitOrbFromQueue

### Type Methods

+ ConnectToDeviceStatic

+ CriticalOrbSubmissionStatic

+ FetchAgentResetCompleteStatic

+ LoginCompletionStatic

+ LogoutCompletionStatic

+ LunResetCompleteStatic

+ StatusNotifyStatic

+ UnsolicitedStatusNotifyStatic

## Relationships

### Inherits From

- IOSCSIProtocolServices

## See Also

### Interfaces

IOFireWireSBP2Target

Serves as bridge between IOFireWireUnit and IOFireWireLUN.

IOFireWireController

IOFireWireBus

IOFireWireBus is a public class the provides access to general FireWire functionality...

