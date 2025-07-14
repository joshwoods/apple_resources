

- Kernel
- Hardware Families
- Audio
- IOAudioControl
-  newUserClient 

# newUserClient

Creates a new user client object for this IOAudioControl instance.

``` source
virtual IOReturn newUserClient(
 task_t task,
 void *securityID,
 UInt32 type,
 IOUserClient **handler); 
```

## Parameters 

`task`  

The task requesting the new user client.

`securityID`  

Optional security paramater passed in by the client - ignored.

`type`  

Optional user client type passed in by the client - 0 for the default user client type.

`handler`  

The new IOUserClient \* must be stored in this param on a successful completion.

`properties`  

A dictionary of additional properties for the connection.

## Return Value

Returns kIOReturnSuccess on success. May also result kIOReturnError or kIOReturnNoMemory.

## Overview

This is called automatically by I/O Kit when a user process opens a connection to this IOAudioControl. This is typically done when the user process needs to register for value change notifications. This implementation allocates a new IOAudioControlUserClient object. There is no need to call this directly. A derived class that requires overriding of newUserClient should override the version with the properties parameter for Intel targets, and without the properties parameter for PPC targets. The \#if \_\_i386\_\_ directive can be used to select between the two behaviors.

## See Also

### Miscellaneous

addUserClient

Called on the IOWorkLoop to add a new IOAudioControlUserClient.

addUserClientAction

IOCommandGate Action which calls addUserClient() while holding the IOCommandGate.

clientClosed

Called automatically by the IOAudioControlUserClient when a user client closes its connection to the control.

createUserClient(task_t, void *, UInt32, IOAudioControlUserClient **)

Creates a new IOAudioControlUserClient instance.

createUserClient(task_t, void *, UInt32, IOAudioControlUserClient **, OSDictionary *)

Creates a new IOAudioControlUserClient instance.

detachUserClientsAction

flushValue

Forces the control to be flushed out to the hardware.

free

Frees all of the resources allocated by the IOAudioControl.

getChannelID

Returns the channel ID for the control.

getCommandGate

Returns the IOCommandGate for this IOAudioControl.

getControlID

Returns the control ID for the control.

getIsStarted

Returns true after start() has been called.

getValue

Returns the current value of the control.

getWorkLoop

Returns the IOWorkLoop for the whole audio driver.

hardwareValueChanged

Updates the value for this control and sends out the value changed notification.

init

Initializes a newly allocated IOAudioControl with the given attributes.

performValueChange

Called by setValue() to make the call to the valueChangeHandler to update the hardware.

removeUserClient

Called on the IOWorkLoop to remove an IOAudioControlUserClient.

removeUserClientAction

IOCommandGate Action which calls removeUserClient() while holding the IOCommandGate.

sendValueChangeNotification

Called when the value has changed for the control.

setChannelID

Called at init time to set the channel ID for this IOAudioControl.

setChannelName

Called at init time to set the channel name for this IOAudioControl.

setControlID

Sets the controlID for this control.

setProperties

Changes a property of this IOService.

setReadOnlyFlag

Call this function to say that a control is read only. This call cannot be undone, so if a control is only temporarily unsetable, do not use this call but instead return an error from the control handler.

setSubType(UInt32)

Called at init time to set the control type.

setType(UInt32)

Called at init time to set the control type.

setUsage

Called at init time to set the control usage.

setValue

Sets the value for this control.

setValueAction

IOCommandGate Action which calls setValue() while holding the IOCommandGate.

start

Starts a newly created IOAudioControl.

stop

Stops the control when the provider is going away.

updateValue

Called by setValue() in order to update the value and the registry.

validateValue

Called by setValue() to verify that the value is valid.

withAttributes

Static function that allocates a new IOAudioControl with the given attributes.

