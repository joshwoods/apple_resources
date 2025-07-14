

- Kernel
- Hardware Families
- SCSI
- IOSCSIParallelInterfaceController
-  TerminateController 

# TerminateController

Called to terminate the controller

``` source
virtual void TerminateController (
 void ) = 0; 
```

## Overview

It is guaranteed that the TerminateController() will only be called once and only after the InitializeController() method and only if true was returned in response to the InitializeController() method. The TerminateController() method allows the subclass to release all resources that were acquired for operation of the hardware and shutdown all hardware services. This is the last method of the subclass that will be called before the class is destroyed.

## See Also

### Miscellaneous

CompleteParallelTask

Parallel Task Completion

CreateDeviceInterrupt

Called to create an IOInterruptEventSource for the device. Subclasses may wish to use a different interrupt index than 0 (e.g. for using PCI Message Signaled Interrupts) or might not need an interrupt at all (virtual HBA).

CreateTargetForID(SCSIDeviceIdentifier)

Method to perform device creation.

CreateTargetForID(SCSIDeviceIdentifier, OSDictionary *)

Method to perform device creation.

DestroyTargetForID

Method to perform device destruction.

DisableInterrupt

Disable Interrupt

DoesHBAPerformAutoSense

Queries the HBA child class to determine if it automatically performs AutoSense and provides AutoSense data for each I/O. If the HBA allocates space for AutoSense in its HBA specific data region on a per task basis, the HBA should respond true.

DoesHBAPerformDeviceManagement

Determine if HBA will manage devices.

DoesHBASupportMultiPathing

Queries the HBA child class to determine if it supports Multi-Pathing.

DoesHBASupportSCSIParallelFeature

Queries the HBA child class to determine if it supports a specific SPI feature.

EnableInterrupt

Enable Interrupt

ExecuteParallelTask

Submit a SCSIParallelTask for execution.

FilterInterruptRequest

Filter method called at primary interrupt time.

FindTaskForAddress

Find a task for a given Task Address, if one exists.

FindTaskForControllerIdentifier

Find a task for a given Target and Controller Task Identifier

FreeSCSIParallelTask

Method to allow the client to release a SCSIParallelTask

GetAutoSenseData

Method to retrieve auto sense data buffer associated with a request.

GetAutoSenseDataSize

Method to retrieve auto sense data buffer size associated with a request.

GetCommandDescriptorBlock

Method to retrieve the SCSI Command Descriptor Block (CDB).

GetCommandDescriptorBlockSize

Method to retrieve the size of the SCSI Command Descriptor Block (CDB).

GetCommandGate

Accessor to get an IOCommandGate associated with the workloop.

GetDataBuffer

Method to retrieve client buffer from the request.

GetDataBufferOffset

Method to retrieve offset into client buffer at which to start processing.

GetDataTransferDirection

Retrieves the data transfer direction for any data associated with the request.

GetDMACommand

Method to retrieve a pointer to an IODMACommand from the request.

GetHBADataDescriptor

Method to retrieve the IOMemoryDescriptor associated with the HBA Data.

GetHBADataPointer

Method to retrieve the HBA Data pointer.

GetHBADataSize

Method to retrieve the HBA Data Size in bytes.

GetHBATargetDataPointer

Method to retrieve the HBA Data pointer.

GetHBATargetDataSize

Method to retrieve the HBA Data Size in bytes.

GetLogicalUnitBytes

Method to get the logical unit bytes associated with a request.

GetLogicalUnitNumber

Method to get the logical unit number associated with a request.

GetProvider

Accessor method to get the IOService which is the controller's provider.

GetRealizedDataTransferCount

Retrieves the realized data transfer count for any data associated with the request.

GetRequestedDataTransferCount

Retrieves the requested data transfer count for any data associated with the request.

GetSCSIDomainIdentifier

Accessor method to get the SCSI Domain Identifier.

GetSCSIParallelFeatureNegotiation

Method to retrieve the requested value for negotiation of the.

GetSCSIParallelFeatureNegotiationCount

Method to retrieve the number of requested negotiations.

GetSCSIParallelFeatureNegotiationResult

Method to retrieve the result of any wide transfer negotiations.

GetSCSIParallelFeatureNegotiationResultCount

Method to retrieve the number of changed negotiations.

GetSCSIParallelTask

Method to allow the client to get a SCSIParallelTask

GetSCSITaskIdentifier

Method to retrieve a SCSITaskIdentifier from a valid SCSIParallelTaskIdentifier.

GetTaggedTaskIdentifier

Method to retrieve the SCSI Tagged Task Identifier of the task. If the returned value is equal to kSCSIUntaggedTaskIdentifier, then this task is untagged.

GetTargetForID

Accessor for getting pointer to IOSCSIParallelInterfaceDevice.

GetTargetIdentifier

Method to get the SCSITargetIdentifier associated with a request.

GetTaskAttribute

Method to retrieve the SCSI Task Attribute of the task

GetTimeoutDuration

Method to retrieve the timeout duration in milliseconds for a request.

GetWorkLoop

Accessor method to get the IOWorkLoop associated with this HBA.

HandleInterruptRequest

Handle Interrupt Request

HandleTimeout

Method to handle command timeouts.

IncrementRealizedDataTransferCount

Increments the realized data transfer count. This method is helpful for when the HBA has to do multiple passes of DMA because there are more scatter-gather elements than it can process in one pass.

InitializeController

Called to initialize the controller

InitializeDMASpecification

Called to initialize an IODMACommand with a DMA specification.

InitializeTargetForID

Called to initialize a target device.

NotifyClientsOfBusReset

Method called to notify clients that a bus reset has occurred.

NotifyClientsOfPortStatusChange

Method called to notify clients of port status change events.

ProcessParallelTask

Called by client to process a parallel task.

RemoveHBAProperty

Accessor for removing a property for this object.

RemoveTargetProperty

Accessor for removing a property from a specific target.

ReportHBAConstraints

Called to report the I/O constraints for this controller. A list of valid keys includes: kIOMaximumSegmentCountReadKey, (required) kIOMaximumSegmentCountWriteKey, (required) kIOMaximumSegmentByteCountReadKey, (required) kIOMaximumSegmentByteCountWriteKey, (required) kIOMinimumSegmentAlignmentByteCountKey, (required) kIOMaximumSegmentAddressableBitCountKey, (required) kIOMinimumHBADataAlignmentMaskKey (required) kIOHierarchicalLogicalUnitSupportKey (optional). NB: These keys and their values are described in this header and \

ReportHBAHighestLogicalUnitNumber

Gets the Highest Logical Unit Number.

ReportHBASpecificDeviceDataSize

Determine memory needed for HBA Device specific use.

ReportHBASpecificTaskDataSize

Determine memory needed for HBA Task specific use.

ReportHighestSupportedDeviceID

Get the highest supported SCSI Device Identifier.

ReportInitiatorIdentifier

Get the SCSI Device Identifier for the HBA.

ReportMaximumTaskCount

Report Maximum Task Count

ResumeServices

Called to resume controller services

SetAutoSenseData

Method to set the auto sense data buffer associated with a request.

SetControllerTaskIdentifier

Method to set the Controller Task Identifier.

SetHBAProperty

Accessor for setting a property for this object.

SetRealizedDataTransferCount

Sets the realized data transfer count in bytes.

SetSCSIParallelFeatureNegotiationResult

Method to set the wide data transfer negotiation result.

SetTargetProperty

Accessor for setting a property for a specific target.

SetTimeoutForTask

Method to set the timeout duration in milliseconds for a request.

SignalInterrupt

Signals that an interrupt has occurred.

StartController

Called to start the controller

StopController

Called to stop the controller

SuspendServices

Called to suspend controller services

