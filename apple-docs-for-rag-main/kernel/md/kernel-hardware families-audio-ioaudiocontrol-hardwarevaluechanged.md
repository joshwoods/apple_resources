

- Kernel
- Hardware Families
- Audio
- IOAudioControl
-  hardwareValueChanged 

# hardwareValueChanged

Updates the value for this control and sends out the value changed notification.

``` source
virtual IOReturn hardwareValueChanged(
 OSObject *newValue); 
```

## Parameters 

`newValue`  

The new value for this control.

## Return Value

Returns kIOReturnSuccess if the value is successfully updated.

## Overview

This is designed to be called by the driver when it detects that the hardware's value has changed without driver intervention (e.g. when an external event causes the change). The difference between hardwareValueChanged() and setValue() is that hardwareValueChanged() doesn't call performValueChange() which sends a message back to the driver to cause it to change the hardware with the new value. This function must be called on the IOWorkLoop.

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

init

Initializes a newly allocated IOAudioControl with the given attributes.

newUserClient

Creates a new user client object for this IOAudioControl instance.

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

