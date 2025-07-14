

- Kernel
- Hardware Families
- Audio
-  IOAudioDevice 

Class

# IOAudioDevice

Abstract base class for a single piece of audio hardware. The IOAudioDevice provides the central coordination point for an audio driver.

macOS 10.1+

``` source
class IOAudioDevice : IOService
```

## Overview

An audio driver is required to subclass IOAudioDevice in order to provide working audio to the system. A single driver instance will contain a single instance of the driver's IOAudioDevice subclass. The subclass is responsible for mapping all hardware device resources from the service provider nub. It must control access to the hardware so that the hardware doesn't get into an inconsistent state. It is possible that different threads may make requests of the hardware at the same time. The IOAudioDevice superclass provides an IOWorkLoop and IOCommandGate on the IOWorkLoop through which all hardware accesses may be synchronized. All entry points to all parts of the driver controlled by the IOAudioFamily will be synchronized through this one IOWorkLoop.

The IOAudioDevice subclass is responsible for creating the rest of the pieces of the driver. It must identify and create all IOAudioEngines that are not automatically created by the system (i.e. those that are not matched and instantiated by IOKit directly).

The IOAudioDevice subclass must enumerate and create all IOAudioControls to match the device capabilities.

It must also execute control value chages when requested by the system (i.e. volume adjustments).

In order to allow sleep and wake to work on the system, the IOAudioDevice subclass is responsible for performing the necessary actions to sleep and wake its hardware (and restore necessary state on wake).

The IOAudioDevice class provides timer services that allow different elements in the audio driver to receive timer notifications as needed. These services were designed with the idea that most timed events in a typical audio driver need to be done at least as often as a certain interval. Further, it is designed with the idea that being called more often than the specified interval doesn't hurt anything - and in fact may help. With this in mind, the timer services provided by the IOAudioDevice class allow different targets to register for timer callbacks at least as often as the specified interval. The actual interval will be the smallest of the intervals of all of the callbacks. This way, we avoid the overhead of having many timers in a single audio device. As an example, each output IOAudioEngine has a timer to run the erase head. It doesn't hurt to have the erase head run more often. Also, a typical IOAudioDevice subclass may need to run a timer to check for device state changes (e.g. jack insertions).

There are a number of strings passed from the driver to the CoreAudio.framework and then into applications. All of those strings should be localized by the driver. In order to do that the kext bundle should have localized string files following the macOS localization instructions. The IOAudioDevice should contain a property with the name of the bundle/kext that contains the localized string resources. To do that, the driver's personality in the bundle resources could have a property named 'IOAudioDeviceLocalizedBundle' with the path of the bundle/kext relative to '/System/Library/Extensions'. It could also be set by the IOAudioDevice subclass in its initHardware() function. To do so, call setProperty(kIOAudioDeviceLocalizedBundleKey, "Driver.kext").

In a typical driver, the IOAudioDevice subclass will implement initHardware() to perform the hardware initialization and driver construction. Within that initialization it must create at least one IOAudioEngine instance and activate it. In order to activate a new IOAudioEngine activateAudioEngine() should be called for each one. It must create the IOAudioControls matching the hardware capabilities to allow the system to set volume, mute and input selection. To add those controls to the driver, each control should be attached to the IOAudioEngine to which it applies by calling addDefaultAudioControl() on the IOAudioEngine. During initialization it should also call setDeviceName(), setDeviceShortName() and setManufacturerName() with localized strings representing each of the attributes.

If the driver is to work properly after sleep/wake, it must implement performPowerStateChange() and deal with the sleep and wake transitions. It may also deal with the idle state transitions to turn off device power when it isn't in use (especially useful for devices attached to a portable running on battery power).

## Topics

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

### Callbacks

TimerEvent

Generic timer event callback for IOAudioDevice timer targets

### Constants

gIOAudioPlane

### Instance Variables

workLoop

timerEventSource

timerEvents

The set of timer events in use by the device.

pendingPowerState

numRunningAudioEngines

minimumInterval

familyManagePower

duringStartup

currentPowerState

commandGate

audioPorts

audioEngines

asyncPowerStateChangeInProgress

### Instance Methods

- activateAudioEngineDeprecated

- activateAudioEngineDeprecated

- addTimerEventDeprecated

- attachAudioPortDeprecated

- audioEngineStartingDeprecated

- audioEngineStoppedDeprecated

- completePowerStateChangeDeprecated

- deactivateAllAudioEnginesDeprecated

- detachAllAudioPortsDeprecated

- dispatchTimerEventsDeprecated

- flushAudioControlsDeprecated

- freeDeprecated

- getCommandGateDeprecated

- getMetaClass

- getPendingPowerStateDeprecated

- getPowerStateDeprecated

- getWorkLoopDeprecated

- initDeprecated

- initHardwareDeprecated

- initiatePowerStateChangeDeprecated

- performPowerStateChangeDeprecated

- protectedCompletePowerStateChangeDeprecated

- protectedSetPowerStateDeprecated

- removeAllTimerEventsDeprecated

- removeTimerEventDeprecated

- scheduleIdleAudioSleepDeprecated

- setAggressivenessDeprecated

- setConfigurationApplicationBundleDeprecated

- setDeviceCanBeDefaultDeprecated

- setDeviceModelNameDeprecated

- setDeviceNameDeprecated

- setDeviceShortNameDeprecated

- setDeviceTransportTypeDeprecated

- setFamilyManagePowerDeprecated

- setIdleAudioSleepTimeDeprecated

- setManufacturerNameDeprecated

- setPowerStateDeprecated

- startDeprecated

- stopDeprecated

- waitForPendingPowerStateChangeDeprecated

- willTerminateDeprecated

### Type Methods

+ completePowerStateChangeActionDeprecated

+ idleAudioSleepHandlerTimerDeprecated

+ setPowerStateActionDeprecated

+ timerFiredDeprecated

## Relationships

### Inherits From

- IOService

