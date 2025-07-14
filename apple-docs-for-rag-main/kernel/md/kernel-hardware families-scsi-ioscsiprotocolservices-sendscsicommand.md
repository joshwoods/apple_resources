

- Kernel
- Hardware Families
- SCSI
- IOSCSIProtocolServices
-  SendSCSICommand 

# SendSCSICommand

Pure virtual method subclasses must implement in order to send SCSITasks on the wire.

``` source
virtual bool SendSCSICommand (
 SCSITaskIdentifierrequest, 
 SCSIServiceResponse *serviceResponse, 
 SCSITaskStatus *taskStatus ) = 0; 
```

## Parameters 

`request`  

A valid SCSITaskIdentifier representing the command to send on the wire.

`serviceResponse`  

Pointer to a SCSIServiceResponse value returned to the caller.

`taskStatus`  

Pointer to a SCSITaskStatus value returned to the caller.

## Return Value

False if no more commands can be processed at this time, otherwise true.

## Overview

Send a SCSI Command to the device. If the command was sent to the device and is pending completion, the subclass should return true and return back the kSCSIServiceResponse_Request_In_Process response. If the command completes immediately with an error, the subclass will return true and return back the appropriate status. If the subclass is currently processing all the commands it can, the subclass will return false and the command will be resent next time CommandCompleted is called.

## See Also

### Miscellaneous

AbortCommand

Deprecated. Do not use.

AbortSCSICommand

Pure virtual method subclasses must implement so that SCSITasks may be aborted.

AbortSCSITaskFromQueue

Deprecated internal method.

AbortTask

The Task Management function to allow the SCSI Application Layer client to request that a specific task be aborted.

AbortTaskSet

The Task Management function to allow the SCSI Application Layer client to request that a complete task set be aborted.

AddSCSITaskToHeadOfQueue

Internal method called to add a SCSITask to the head of the processing queue.

AddSCSITaskToQueue

Internal method called to add a SCSITask to the processing queue.

ClearACA

The Task Management function to clear an Auto-Contingent Allegiance condition.

ClearTaskSet

The Task Management function to clear a task set.

CommandCompleted

Method subclass calls to complete a SCSITask.

CreateSCSITargetDevice

Used to create a SCSITargetDevice which will manage logical units.

EnsureAutosenseDescriptorExists

Internal method, not to be called by subclasses.

ExecuteCommand

ExecuteCommand method will take a SCSI Task and transport it across the physical wire(s) to the device.

free

Frees data structures that were allocated during start().

GetAutosenseRequestedDataTransferCount

Accessor method to retrieve the requested data transfer count for autosense data associated with the specified request.

GetCommandDescriptorBlock

Accessor method to retrieve the Command Descriptor Block associated with the specified request.

GetCommandDescriptorBlockSize

Accessor method to retrieve the Command Descriptor Block size associated with the specified request.

GetDataBuffer

Accessor method to retrieve the data buffer associated with the specified request.

GetDataBufferOffset

Accessor method to retrieve the data buffer offset associated with the specified request.

GetDataTransferDirection

Accessor method to retrieve the data transfer direction associated with the specified request.

GetInitialPowerState

This method is called once, right after InitializePowerManagement() in order to determine what state the device is initially in at startup time (usually the highest power mode).

GetLogicalUnitBytes

Accessor method to retrieve the logical unit bytes associated with the specified request.

GetLogicalUnitNumber

Accessor method to retrieve the logical unit number associated with the specified request.

GetProtocolLayerReference

Accessor method to retrieve the protocol layer reference.

GetRealizedDataTransferCount

Accessor method to retrieve the realized data transfer count associated with the specified request.

GetRequestedDataTransferCount

Accessor method to retrieve the requested data transfer count associated with the specified request.

GetTaskAttribute

Accessor method to retrieve the SCSITaskAttribute associated with the specified request.

GetTaskExecutionMode

Internal method used to retrieve the task execution mode.

GetTaskState

Accessor method to retrieve the SCSITaskState associated with the specified request.

GetTimeoutDuration

Accessor method to retrieve the timeout duration in milliseconds associated with the specified request.

HandleAbortTask

HandleAbortTask instructs the Protocol Services driver to abort the task.

HandleAbortTaskSet

HandleAbortTaskSet instructs the Protocol Services driver to abort the task set.

HandleCheckPowerState

Method called to check if the device is in the correct power state for an I/O.

HandleClearACA

HandleClearACA instructs the Protocol Services driver to clear an auto-contingent allegiance.

HandleClearTaskSet

HandleClearTaskSet instructs the Protocol Services driver to clear the task set.

HandleLogicalUnitReset

HandleLogicalUnitReset instructs the Protocol Services driver to reset the logical unit.

HandlePowerChange

This method is called to handle a power change.

HandlePowerOff

Convenience method for a protocol service driver to handle a power off call (called on the way to sleep).

HandlePowerOn

Convenience method for a protocol service driver to handle a power on call (called on the way back up from sleep).

HandleProtocolServiceFeature

HandleProtocolServiceFeature instructs the Protocol Services driver to perform the necessary tasks for the indicated feature.

HandleTargetReset

HandleTargetReset instructs the Protocol Services driver to reset the target.

init

Standard init method for all IORegistryEntry subclasses.

InitializePowerManagement

Subclasses call this method to initialize power management.

IsProtocolServiceSupported

IsProtocolServiceSupported will return true if the specified feature is supported by the protocol layer.

LogicalUnitReset

The Task Management function to reset a logical unit.

ProcessCompletedTask

Internal method called to process completed SCSITasks.

RegisterSCSITaskCompletionRoutine

Used by IOSCSITargetDevice to register a completion routine.

RejectSCSITasksCurrentlyQueued

Internal method called to reject currently enqueued SCSITasks.

RejectTask

Internal method called to reject a particular SCSITask.

RetrieveNextSCSITaskFromQueue

Internal method called to retrieve the next SCSITask to process.

SendNotification_DeviceRemoved

Method called by subclasses when a device is physically removed from the bus.

SendNotification_VerifyDeviceState

Method called by subclasses when a device state needs to be re-verified due to some bus condition which may have changed the device state.

SendSCSITasksFromQueue

Internal method called to start processing SCSITasks.

SetAutoSenseData(SCSITaskIdentifier, SCSI_Sense_Data *)

Accessor method to set the autosense data. NOTE: This method is deprecated.

SetAutoSenseData(SCSITaskIdentifier, SCSI_Sense_Data *, UInt8)

Accessor method to set the autosense data.

SetProtocolLayerReference

Accessor method to set the protocol layer reference.

SetRealizedDataTransferCount

Accessor method to set the realized (actual) data transfer count associated with the specified request.

SetTaskExecutionMode

Internal method used to set the task execution mode.

SetTaskState

Accessor method to set the SCSITaskState associated with the specified request.

start

During an IOService object's instantiation, starts the IOService object that has been selected to run on the provider.

TargetReset

The Task Management function to reset a target device.

TicklePowerManager

Internal method. Do not use.

