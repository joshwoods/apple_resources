

- Kernel
- Hardware Families
- Audio
- IOAudioDevice
-  activateAudioEngine(IOAudioEngine \*, bool) 

# activateAudioEngine(IOAudioEngine \*, bool)

This is called to add a new IOAudioEngine object to the IOAudioDevice.

``` source
virtual IOReturn activateAudioEngine(
 IOAudioEngine *audioEngine,
 boolshouldStartAudioEngine); 
```

## Parameters 

`audioEngine`  

The IOAudioEngine instance to be activated.

`shouldStartAudioEngine`  

If true, the audio engine is treated as a newly allocated IOAudioEngine instance and is appropriately attached and started according to IOKit convention. If it is false it is assumed that some other process (possibly the IOKit matching process) has started the IOAudioEngine and will skip that step.

## Return Value

Returns true if the audio engine was successfully activated.

## Overview

Once the IOAudioEngine has been activated by this function, it is ready to begin moving audio data. This should be called either during the subclass' initHardware() implementation for each IOAudioEngine the device creates. Or it should be called by the IOAudioEngine itself if the audio engine was automatically created by IOKit's matching process. The system won't be able to properly track and control IOAudioEngines if they are not activated though this function. This implementation will retain the IOAudioEngine while it maintains control of it. When the audio engine is deactivated, the IOAudioEngine will be released. If the IOAudioDevice subclass is passing a newly instantiated IOAudioEngine, it will need to release the audio engine after it has been activated. This will insure that the refCount on the audio engine is correct when it gets deactivated when the driver is stopped. That allows the audio engine to be freed when it is no longer needed.

## See Also

### Miscellaneous

activateAudioEngine(IOAudioEngine *)

This simply calls activateAudioEngine(IOAudioEngine \*audioEngine, bool shouldStartAudioEngine) with a value of true for shouldStartAudioEngine.

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

performPowerStateChange

This function is called by the IOAudioDevice when a power state change is needed.

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

