

- SCSIControllerDriverKit
-  IOUserSCSIParallelInterfaceController 

Class

# IOUserSCSIParallelInterfaceController

A DriverKit provider object that manages communications with SCSI-based devices.

DriverKit

``` source
class IOUserSCSIParallelInterfaceController;
```

## Overview

Implement your driver by subclassing this class and overriding all pure virtual methods.

### Specifying the Driver’s Personality Information

When you subclass `IOUserSCSIParallelInterfaceController`, update the IOKitPersonalities key of your driver extension’s `Info.plist` file with information to match your driver to appropriate hardware. For this class, always include the keys and values in the following table:

| Key                      | Value                                   |
|--------------------------|-----------------------------------------|
| IOClass                  | `IOUserSCSIParallelInterfaceController` |
| IOUserClass              | The name of your custom dext class.     |
| IOProviderClass          | `IOPCIDevice`                           |
| CFBundleIdentifierKernel | `com.apple.iokit.IOSCSIParallelFamily`  |

### Supporting Power Capabilities

IOUserSCSIParallelInterfaceController supports the following power capabilities:

- kIOServicePowerCapabilityOff

- kIOServicePowerCapabilityOn

- kIOServicePowerCapabilityPause

Implement the SetPowerState method in your service object and use it to put your driver in a safe state for the new power setting. Call `super` either as the last step in your implementation, or when the dext is ready to acknowledge the power state transition.

The following code example implements SetPowerState by performing a check to see if the new state is kIOServicePowerCapabilityOn. If it is, the implementation calls a private `IssueHardReset()` method.

```
```

The hypothetical driver in this example still needs to acknowledge the power state change when it’s appropriate. For example, it could ensure a rescan has brought up all its targets, and then call `SetPowerState ( powerState, SUPERDISPATCH );`.

## Topics

### Managing Controllers

UserInitializeController

Initializes the controller in response to a call from the framework.

UserStartController

Starts the controller in response to a call from the framework.

### Managing Tasks

UserProcessParallelTask

Processes a parallel task in response to a call from the framework.

SCSIUserParallelTask

The properties of a parallel task to perform.

ParallelTaskCompletion

Indicates to the system that the extension has completed an asynchronous request.

SCSIUserParallelResponse

The properties of a completed request.

### Managing Bundled Parallel Tasks

UserProcessBundledParallelTasks

Processes one or more parallel tasks in response to a call from the framework.

UserMapBundledParallelTaskCommandAndResponseBuffers

Maps the shared command and response buffers in the dext address space in response to a call from the framework.

BundledParallelTaskCompletion

Indicates to the system that the extension completed a bundled asynchronous request.

### Managing Targets

UserInitializeTargetForID

Initializes a target device in response to a call from the framework.

UserCreateTargetForID

Creates the specified target.

UserDestroyTargetForID

Destroys the specified target.

UserTargetPresentForID

Checks if a specific target is present.

UserSetTargetProperties

Sets properties on the target.

UserRemoveTargetProperties

Removes properties from a target.

### Performing SCSI Standard Task Management

UserAbortTaskRequest

Aborts a single task.

UserAbortTaskSetRequest

Aborts all tasks in a logical unit.

UserClearACARequest

Removes an autocontingent allegiance (ACA) attribute from a logical unit’s task set.

UserClearTaskSetRequest

Aborts all tasks in a logical unit and clears their data.

UserLogicalUnitResetRequest

Resets a logical unit.

UserTargetResetRequest

Resets a target.

### Managing Host Bus Adapters

UserReportInitiatorIdentifier

Gets the SCSI device identifier for the host bus adapter (HBA) in response to a call from the framework.

UserReportHighestSupportedDeviceID

Gets the highest supported SCSI device identifier in response to a call from the framework.

UserReportMaximumTaskCount

Gets the maximum number of outstanding tasks the HBA can process in response to a call from the framework.

UserDoesHBAPerformDeviceManagement

Determines if the host bus adapter (HBA) manages devices in response to a call from the framework.

UserReportHBAHighestLogicalUnitNumber

Gets the highest logical unit number (LUN) in response to a call from the framework.

UserDoesHBAPerformAutoSense

Determines if the driver extension class automatically performs autosense and provides autosense data for each I/O in response to a call from the framework.

UserDoesHBASupportMultiPathing

Queries the HBA child class to determine if it supports multipathing in response to a call from the framework.

UserDoesHBASupportSCSIParallelFeature

Determines whether the driver extension class supports a specific feature in response to a call from the framework.

SCSIParallelFeature

A feature that the driver extension supports.

UserMapHBAData

Maps any host bus adapter (HBA)-specific task data in response to a call from the framework.

UserSetHBAProperties

Sets multiple properties for a host bus adapter.

UserRemoveHBAProperties

Removes properties from a host bus adapter in response to a call from the framework.

UserReportHBAConstraints

Reports the I/O constraints for this controller.

### Managing Direct Memory Access

UserGetDMASpecification

Gets the controller-specific direct memory access (DMA) specification in response to a call from the framework.

DMAOutputSegmentType

The size and endianness that the system uses for direct memory access (DMA).

### Supporting SCSI Power States

kIOServicePowerCapabilityPause

A PCIe-specific power state for halting transactions while reallocating resources.

### Instance Methods

UserCallMediaParametersHaveChanged

UserGetDataBuffer

## Relationships

### Inherits From

- IOService

