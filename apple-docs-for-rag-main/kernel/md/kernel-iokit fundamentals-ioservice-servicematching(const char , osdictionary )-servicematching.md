

- Kernel
- IOKit Fundamentals
- IOService
-  serviceMatching(const char \*, OSDictionary \*) 

# serviceMatching(const char \*, OSDictionary \*)

Creates a matching dictionary, or adds matching properties to an existing dictionary, that specify an IOService class match.

``` source
static OSDictionary * serviceMatching(
 const char *className, 
 OSDictionary *table = 0 ); 
```

## Parameters 

`className`  

The class name, as a const C string. Class matching is successful on IOService objects of this class or any subclass.

`table`  

If zero, `serviceMatching` creates a matching dictionary and returns a reference to it, otherwise the matching properties are added to the specified dictionary.

## Return Value

The matching dictionary created, or passed in, is returned on success, or zero on failure.

## Overview

A very common matching criteria for IOService object is based on its class. `serviceMatching` creates a matching dictionary that specifies any IOService object of a class, or its subclasses. The class is specified by name, and an existing dictionary may be passed in, in which case the matching properties will be added to that dictionary rather than creating a new one.

## See Also

### Miscellaneous

acknowledgePowerChange

Acknowledges an in-progress power state change.

- acknowledgeSetPowerState

Acknowledges the belated completion of a driver’s setPowerState power state change.

activityTickle

Informs power management when a power-managed device is in use, so that power management can track when it is idle and adjust its power state accordingly.

addLocation

Adds a location matching property to an existing dictionary.

addMatchingNotification

Adds a persistant notification handler to be notified of IOService events.

addNotification

Deprecated use addMatchingNotification(). Adds a persistant notification handler to be notified of IOService events.

addPowerChild

Informs a driver that it has a new child.

adjustBusy

Adjusts the `busyState` of an IOService object.

attach

Attaches an IOService client to a provider in the I/O Registry.

callPlatformFunction

Calls the platform function with the given name.

causeInterrupt

Causes a device interrupt to occur.

changePowerStateTo

Sets a driver's power state.

changePowerStateToPriv

Tells a driver's superclass to change the power state of its device.

clampPowerOn

Deprecated. Do not use.

close

Releases active access to a provider.

command_received

compareProperties

Compares a set of properties in a matching dictionary with an IOService object's property table.

compareProperty(OSDictionary *, const char *)

Compares a property in a matching dictionary with an IOService object's property table.

compareProperty(OSDictionary *, const OSString *)

Compares a property in a matching dictionary with an IOService object's property table.

configureReport

configure IOReporting channels

copyClientWithCategory

copyMatchingService

Finds one of the current published IOService objects matching a matching dictionary.

currentCapability

Finds out the capability of a device's current power state.

currentPowerConsumption

Finds out the current power consumption of a device.

deRegisterInterestedDriver

De-registers power state interest from a previous call to `registerInterestedDriver`.

detach

Detaches an IOService client from a provider in the I/O Registry.

didTerminate

Passes a termination up the stack.

didYouWakeSystem

Asks a driver if its device is the one that just woke the system from sleep.

disableInterrupt

Synchronously disables a device interrupt.

enableInterrupt

Enables a device interrupt.

errnoFromReturn

Translates an IOReturn code to a BSD `errno`.

finalize

Finalizes the destruction of an IOService object.

free

Frees data structures that were allocated when power management was initialized on this service.

getAggressiveness

Returns the current aggressiveness value for the given type.

getBusyState

Returns the `busyState` of an IOService object.

getClient

Returns an IOService object's primary client.

getClientIterator

Returns an iterator over an IOService object's clients.

getDeviceMemory

Returns the array of IODeviceMemory objects representing a device's memory mapped ranges.

getDeviceMemoryCount

Returns a count of the physical memory ranges available for a device.

getDeviceMemoryWithIndex

Returns an instance of IODeviceMemory representing one of a device's memory mapped ranges.

getInterruptType

Returns the type of interrupt used for a device supplying hardware interrupts.

getMatchingServices

Finds the set of current published IOService objects matching a matching dictionary.

getOpenClientIterator

Returns an iterator over a provider's clients that currently have opened the provider.

getOpenProviderIterator

Returns an iterator over an client's providers that are currently opened by the client.

getPlatform

Returns a pointer to the platform expert instance for the computer.

getPMRootDomain

Returns a pointer to the power management root domain instance for the computer.

getPMworkloop

Returns a pointer to the system-wide power management work loop.

getPowerState

Determines a device's power state.

getProvider

Returns an IOService object's primary provider.

getProviderIterator

Returns an iterator over an IOService object's providers.

getResources

Allocates any needed resources for a published IOService object before clients attach.

getResourceService

Returns a pointer to the IOResources service.

getServiceRoot

Returns a pointer to the root of the service plane.

getState

Accessor for IOService state bits, not normally needed or used outside IOService.

getWorkLoop

Returns the current work loop or `provider->getWorkLoop`.

handleClose

Controls the open / close behavior of an IOService object (overrideable by subclasses).

handleIsOpen

Controls the open / close behavior of an IOService object (overrideable by subclasses).

handleOpen

Controls the open / close behavior of an IOService object (overrideable by subclasses).

initialPowerStateForDomainState

Determines which power state a device is in, given the current power domain state.

isInactive

Checks if the IOService object has been terminated, and is in the process of being destroyed.

isOpen

Determines whether a specific, or any, client has an IOService object open.

joinPMtree

Joins the driver into the power plane of the I/O Registry.

lockForArbitration

Locks an IOService object against changes in state or ownership.

makeUsable

Requests that a device become usable.

mapDeviceMemoryWithIndex

Maps a physical range of a device.

matchLocation

Allows a registered IOService object to direct location matching.

matchPropertyTable

Allows a registered IOService object to implement family specific matching.

maxCapabilityForDomainState

Determines a driver's highest power state possible for a given power domain state.

message

Receives a generic message delivered from an attached provider.

messageClient

Sends a generic message to an attached client.

messageClients

Sends a generic message to all attached clients.

nameMatching(const char *, OSDictionary *)

Creates a matching dictionary, or adds matching properties to an existing dictionary, that specify an IOService name match.

nameMatching(const OSString *, OSDictionary *)

Creates a matching dictionary, or adds matching properties to an existing dictionary, that specify an IOService name match.

newTemperature

Tells a power managed driver that the temperature in the thermal zone has changed.

newUserClient

Creates a connection for a non kernel client.

nextIdleTimeout

Allows subclasses to customize idle power management behavior.

open

Requests active access to a provider.

PM_Clamp_Timer_Expired

PM_idle_timer_expiration

PMinit

Initializes power management for a driver.

PMstop

Stop power managing the driver.

powerChangeDone

Tells a driver when a power state change is complete.

powerOverrideOffPriv

Allows a driver to disable a power override.

powerOverrideOnPriv

Allows a driver to ignore its children's power management requests and only use changePowerStateToPriv to define its own power state.

powerStateDidChangeTo

Informs interested parties that a device has changed to a different power state.

powerStateForDomainState

Determines what power state the device would be in for a given power domain state.

powerStateWillChangeTo

Informs interested parties that a device is about to change its power state.

probe

During an IOService object's instantiation, probes a matched service to see if it can be used.

propertyMatching

Creates a matching dictionary, or adds matching properties to an existing dictionary, that specify an IOService phandle match.

publishResource(const char *, OSObject *)

Uses the resource service to publish a property.

publishResource(const OSSymbol *, OSObject *)

Uses the resource service to publish a property.

registerInterestedDriver

Allows an IOService object to register interest in the changing power state of a power-managed IOService object.

registerInterrupt

Registers a C function interrupt handler for a device supplying interrupts.

registerPowerDriver

Registers a set of power states that the driver supports.

registerService

Starts the registration process for a newly discovered IOService object.

registryEntryIDMatching

Creates a matching dictionary, or adds matching properties to an existing dictionary, that specify a IORegistryEntryID match.

removePowerChild

Informs a power managed driver that one of its power plane childen is disappearing.

requestPowerDomainState

Tells a driver to adjust its power state.

requestProbe

Requests that hardware be re-scanned for devices.

requestTerminate

Passes a termination up the stack.

resourceMatching(const char *, OSDictionary *)

Creates a matching dictionary, or adds matching properties to an existing dictionary, that specify a resource service match.

resourceMatching(const OSString *, OSDictionary *)

Creates a matching dictionary, or adds matching properties to an existing dictionary, that specify a resource service match.

serviceMatching(const OSString *, OSDictionary *)

Creates a matching dictionary, or adds matching properties to an existing dictionary, that specify an IOService class match.

setAggressiveness

Broadcasts an aggressiveness factor from the parent of a driver to the driver.

setDeviceMemory

Sets the array of IODeviceMemory objects representing a device's memory mapped ranges.

setIdleTimerPeriod

Sets or changes the idle timer period.

setPowerParent

This call is handled internally by power management. It is not intended to be overridden or called by drivers.

- setPowerState

Requests a power managed driver to change the power state of its device.

start

During an IOService object's instantiation, starts the IOService object that has been selected to run on the provider.

start_PM_idle_timer

stop

During an IOService termination, the stop method is called in its clients before they are detached & it is destroyed.

stringFromReturn

Supplies a programmer-friendly string from an IOReturn code.

systemWake

Tells every driver in the power plane that the system is waking up.

systemWillShutdown

Notifies members of the power plane of system shutdown and restart.

temperatureCriticalForZone

Alerts a driver to a critical temperature in some thermal zone.

temporaryPowerClampOn

A driver calls this method to hold itself in the highest power state until it has children.

terminate

Makes an IOService object inactive and begins its destruction.

terminateClient

Passes a termination up the stack.

unlockForArbitration

Unlocks an IOService obkect after a successful lockForArbitration.

unregisterInterrupt

Removes a C function interrupt handler for a device supplying hardware interrupts.

updateReport

request current data for the specified channels

waitForMatchingService

Waits for a matching to service to be published.

waitForService

Deprecated use waitForMatchingService(). Waits for a matching to service to be published.

waitQuiet

Waits for an IOService object's `busyState` to be zero.

willTerminate

Passes a termination up the stack.

youAreRoot

Informs power management which IOService object is the power plane root.

