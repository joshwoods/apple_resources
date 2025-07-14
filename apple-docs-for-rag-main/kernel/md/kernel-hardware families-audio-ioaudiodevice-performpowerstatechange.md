

- Kernel
- Hardware Families
- Audio
- IOAudioDevice
-  performPowerStateChange 

# performPowerStateChange

This function is called by the IOAudioDevice when a power state change is needed.

``` source
virtual IOReturn performPowerStateChange(
 IOAudioDevicePowerStateoldPowerState, 
 IOAudioDevicePowerStatenewPowerState, 
 UInt32 *microsecondsUntilComplete); 
```

## Parameters 

`oldPowerState`  

The power state before the power state change

`newPowerState`  

The power state being transitioned to

`microsecondsUntilComplete`  

A pointer to a value representing an upper bound on the number of microseconds to complete an asynchronous power state change. It points to a value of zero at the start and if it remains zero, the state change is complete upon a successful return from the function.

## Return Value

Returns kIOReturnSuccess on a successful completion

## Overview

In order to deal with power state changes, a subclass must override this function. Any combination of old and new power states may be passed to this function. If work is to be performed while transitioning to sleep, check for a newPowerState of kIOAudioDeviceSleep. If work is to be performed while transitioning from sleep, check for an oldPowerState of kIOAudioDeviceSleep. A power state of kIOAudioDeviceIdle means the system is awake, but no clients are currently playing or recording audio (i.e. no IOAudioEngines are active). A power state of kIOAudioDeviceActive means that at least one IOAudioEngine is active. It is possible for a power state change to be performed synchronously or asynchronously. In the case of a synchronous power state change, simple leave microsecondsUntilComplete alone and return kIOReturnSuccess. If an asynchronous power state change is needed the driver should do whatever needed to schedule another thread to finish the state change and set the microsecondsUntilComplete to an upper bound on the amount of time it will take to complete the power state change. Then when the power state change is complete, a call must be made to completePowerStateChange(). During an asynchronous power state change, the current power state will remain the same as before the transition began, and the pendingPowerState is set to the new power state that will be set when the change is complete.

## See Also

### Miscellaneous

activateAudioEngine(IOAudioEngine *)

This simply calls activateAudioEngine(IOAudioEngine \*audioEngine, bool shouldStartAudioEngine) with a value of true for shouldStartAudioEngine.

activateAudioEngine(IOAudioEngine *, bool)

This is called to add a new IOAudioEngine object to the IOAudioDevice.

addTimerEvent

Adds a TimerEvent callback for the given target called at least as often as specified in interval.

attachAudioPort

Adds the port to the IOAudioDevice's list of ports and attaches the port to its parent and attaches the child to the port.

audioEngineStarting

Called by IOAudioEngine when it is starting up

audioEngineStopped

Called by IOAudioEngine when it has stopped

completePowerStateChange

Called when a power state change is complete

completePowerStateChangeAction

IOCommandGate Action which calls protectedCompletePowerStateChange() while holding the IOCommandGate.

deactivateAllAudioEngines

Deactivates all of the audio engines in the device.

detachAllAudioPorts

Deactivates all of the ports in the device.

dispatchTimerEvents

Called by timerFired() to cause the timer event callbacks to be called.

flushAudioControls

Forces each IOAudioControl in the driver to have its value flushed out to the hardware. That will cause either the IOAudioControl's ValueChangeHandler to be called.

free

Frees resources used by the IOAudioDevice instance

getCommandGate

Returns the IOCommandGate for this IOAudioDevice

getPendingPowerState

Returns the pending power state if a state change is in progress. Otherwise it returns the current power state change.

getPowerState

Returns the current power state (the old power state if a change is in progress).

getWorkLoop

Returns the IOWorkLoop for the driver

init

Initialize a newly created instance of IOAudioDevice.

initHardware

This function is called by start() to provide a convenient place for the subclass to perform its initialization.

initiatePowerStateChange

Called internally to execute a power state change

protectedCompletePowerStateChange

Called on the IOWorkLoop when a power state change is complete.

protectedSetPowerState

Called by setPowerStateAction() to deal with a power state change from the IOService power management facility.

removeAllTimerEvents

Removes all timer events and stops the timer

removeTimerEvent

Removes the timer event for the given target.

setConfigurationApplicationBundle

This function is to be called if an external configuration application is available to set which application to launch.

setDeviceCanBeDefault

This function is to be called to tell CoreAudio if this device shouldn't be a default device.

setDeviceName

Sets the name of the device

setDeviceShortName

Sets the short name of the device

setFamilyManagePower

Called set whether or not the family should manage the device power throught the IOService power management APIs.

setIdleAudioSleepTime

This function is to be called by a driver that doesn't want to be told about the audio going idle immediately, but at some point in the future.

setManufacturerName

Sets the manufacturer name of the device

setPowerState

Called by the power management system in IOService when the power state of this service needs to change.

setPowerStateAction

IOCommandGate Action which calls protectedSetPowerState() while holding the IOCommandGate

start

This function is called automatically by the system to tell the driver to start vending services to the rest of the system.

stop

This is responsible for stopping the device after the system is done with it (or if the device is removed from the system).

timerFired

Internal static function called when the timer fires.

waitForPendingPowerStateChange

Called internally to wait until a pending power state change is complete.

