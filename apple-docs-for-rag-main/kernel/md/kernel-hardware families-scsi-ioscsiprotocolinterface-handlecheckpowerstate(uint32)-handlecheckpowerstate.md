

- Kernel
- Hardware Families
- SCSI
- IOSCSIProtocolInterface
-  HandleCheckPowerState(UInt32) 

# HandleCheckPowerState(UInt32)

The HandleCheckPowerState(UInt32 maxPowerState) method is called by the subclasses and is passed the maxPowerState number given to the power manager at initialization time. This guarantees the threads block until that power state has been achieved.

``` source
void HandleCheckPowerState (
 UInt32maxPowerState ); 
```

## Parameters 

`maxPowerState`  

The maximum power state in the power state array.

## Overview

The HandleCheckPowerState(UInt32 maxPowerState) method is called by the subclasses and is passed the maxPowerState number given to the power manager at initialization time. This guarantees the threads block until that power state has been achieved.

## See Also

### Miscellaneous

AbortCommand

Obsolete. Do not use this method.

AbortTask

Aborts a task based on the Logical Unit and tagged task identifier.

AbortTaskSet

Aborts a task set based on the Logical Unit.

CheckPowerState

Called by clients to ensure device is in correct power state before issuing I/O.

ClearACA

Clears an Auto-Contingent Allegiance (ACA) for the specified Logical Unit.

ClearTaskSet

Clears a task set for the specified Logical Unit.

ExecuteCommand

Called to send a SCSITask and transport it across the physical wire(s) to the device.

finalize

Finalizes the destruction of an IOService object.

free

Called to release all resources held by the object.

GetCommandGate

Accessor method to obtain the IOCommandGate.

GetInitialPowerState

This method is called to obtain the initial power state of the device (usually the highest).

GetUserClientExclusivityState

Gets the current exclusivity state of the user client.

HandleCheckPowerState()

The HandleCheckPowerState (void) method is on the serialized side of the command gate and can change member variables safely without multi-threading issues. It's main purpose is to call the superclass' HandleCheckPowerState ( UInt32 maxPowerState ) with the max power state the class registered with.

HandleCheckPowerState(void)

The HandleCheckPowerState (void) method is on the serialized side of the command gate and can change member variables safely without multi-threading issues. It's main purpose is to call the superclass' HandleCheckPowerState ( UInt32 maxPowerState ) with the max power state the class registered with.

HandleGetUserClientExclusivityState

Gets the current exclusivity state of the user client.

HandlePowerChange

The HandlePowerChange method is pure virtual and is left to each protocol or application layer driver to implement. It is guaranteed to be called on its own thread of execution and can make synchronous or asynchronous calls.

HandleProtocolServiceFeature

This method is called to enact support of a protocol specific service feature.

HandleSetPowerState

The HandleSetPowerState method is called by the glue code and is on the serialized side of the command gate.

HandleSetUserClientExclusivityState

Sets the current exclusivity state of the user client.

InitializePowerManagement

This method is called to initialize power management.

initialPowerStateForDomainState

Determines which power state a device is in, given the current power domain state.

IsPowerManagementIntialized

Called to determine if power management is initialized.

IsProtocolServiceSupported

This method is called to query for support of a protocol specific service feature.

LogicalUnitReset

Resets the specified Logical Unit.

setPowerState

Requests a power managed driver to change the power state of its device.

SetUserClientExclusivityState

Sets the current exclusivity state of the user client.

sGetPowerTransistionInProgress

The sGetPowerTransistionInProgress method is a static function used as C-\>C++ glue for going behind the command gate.

sGetUserClientExclusivityState

The sGetUserClientExclusivityState method is a static function used as C-\>C++ glue for going behind the command gate.

sHandleCheckPowerState

The sHandleCheckPowerState method is a static function used as C-\>C++ glue for going behind the command gate.

sHandleSetPowerState

The sHandleSetPowerState method is a static function used as C-\>C++ glue for going behind the command gate.

sPowerManagement

The sPowerManagement method is a static C-function which is called using mach's thread_call API. It guarantees us a thread of execution which is different than the power management thread and the workloop thread on which we can issue commands to the device synchronously or asynchronously without worrying about deadlocks. It calls through to HandlePowerChange, which is a state machine used to direct power management.

sSetUserClientExclusivityState

The sSetUserClientExclusivityState method is a static function used as C-\>C++ glue for going behind the command gate.

start

During an IOService object's instantiation, starts the IOService object that has been selected to run on the provider.

TargetReset

Resets the target device.

TicklePowerManager()

The TicklePowerManager(void) method is called by CheckPowerState and sends an activity tickle to the power manager so that the idle timer is reset.

TicklePowerManager(UInt32)

The TicklePowerManager(UInt32 maxPowerState) method is a convenience function which can be called by subclasses in TicklePowerManager (void) in order to tell the power manager to reset idle timer or bring the device into the requested state. It returns whatever is returned by activityTickle (true if device is in the requested state, false if it is not).

TicklePowerManager(void)

The TicklePowerManager(void) method is called by CheckPowerState and sends an activity tickle to the power manager so that the idle timer is reset.

willTerminate

Passes a termination up the stack.

