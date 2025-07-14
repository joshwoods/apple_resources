

- Kernel
- Hardware Families
- Audio
-  IOAudioControl 

Class

# IOAudioControl

Represents any controllable attribute of an IOAudioDevice.

macOS 10.1+

``` source
class IOAudioControl : IOService
```

## Overview

An IOAudioControl instance may belong to one IOAudioPort. Additionally, it may associated with an IOAudioEngine as a default control for that IOAudioEngine.

When its value changes, it sends a notification to the CoreAudio.framework (HAL). It also makes a call to the ValueChangeHandler.

The base IOAudioControl class contains a type, a value and a channel ID representing the channel(s) which the control acts on. It may also contain a readable format for the name of the channel as well as a control ID that can be used to identify unique controls. Additionally it may contain a subType and a usage. Each type has its own set of possible subTypes. There currently four different control types defined: kIOAudioControlTypeLevel, kIOAudioControlTypeToggle, kIOAudioControlTypeSelector. Each one is represented by a subclass of IOAudioControl: IOAudioLevelControl, IOAudioToggleControl, IOAudioSelectorControl. The level control defines a range of allowed values and has a defined subtype of kIOAudioLevelControlSubTypeVolume used to define a volume control. The toggle control allows for a boolean value and has a defined subtype kIOAudioToggleControlSubTypeMute for a mute control. The selector control has a list of allowed selections with a value and description for each allowed selection and has the following sub types: kIOAudioSelectorControlSubTypeOutput for an output selector and kIOAudioSelectorControlSubTypeInput for an input selector. See the subclass documentation for a more complete description of each

There are enums for default channel ID values and common channel names in IOAudioTypes.h. The channel ID values are prefixed with 'kIOAudioControlChannelID' and the common channel names are prefixed with 'kIOAudioControlChannelName'. All of the attributes of the IOAudioControl are stored in the registry. The key used for each attribute is defined in IOAudioTypes.h with the define matching the following pattern: 'kIOAudioControl\Key'. For example: kIOAudioControlChannelIDKey.

In addition to the existing defined control types, drivers can define their own as well for other purposes.

Changes to the IOAudioControl's value made by the CoreAudio.framework are done through the IORegistry. When the CoreAudio.framework initiates a value change, the control receives a setProperties() message. The setProperties() implementation looks for the property 'IOAudioControlValue' and if present, calls setValue() on the driver's IOWorkLoop with the new value. The setValue() function first checks to see if the new value is different. If so, it calls performValueChange() to call through to the driver to make the change in the hardware. If that call succeeds the value is changed and the new value is set in the registry. Additionally notifications are sent to all clients that have registered for them.

## Topics

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

### Callbacks

IntValueChangeHandler

Handler function used to make a notification when a value is to be changed.

### Instance Variables

workLoop

userClients

isStarted

controlID

commandGate

channelID

### Instance Methods

- addUserClientDeprecated

- attachAndStartDeprecated

- clientClosedDeprecated

- createUserClientDeprecated

- createUserClientDeprecated

- detachUserClientsDeprecated

- flushValueDeprecated

- freeDeprecated

- getChannelIDDeprecated

- getCommandGateDeprecated

- getControlIDDeprecated

- getDataBytesDeprecated

- getDataLengthDeprecated

- getIntValueDeprecated

- getIsStartedDeprecated

- getMetaClass

- getSubTypeDeprecated

- getTypeDeprecated

- getUsageDeprecated

- getValueDeprecated

- getWorkLoopDeprecated

- hardwareValueChangedDeprecated

- initDeprecated

- newUserClientDeprecated

- newUserClientDeprecated

- performValueChangeDeprecated

- removeUserClientDeprecated

- sendChangeNotificationDeprecated

- sendQueuedNotificationsDeprecated

- sendValueChangeNotificationDeprecated

- setChannelIDDeprecated

- setChannelNameDeprecated

- setChannelNumberDeprecated

- setControlIDDeprecated

- setCoreAudioPropertyIDDeprecated

- setPropertiesDeprecated

- setReadOnlyFlagDeprecated

- setSubTypeDeprecated

- setTypeDeprecated

- setUsageDeprecated

- setValueDeprecated

- setValueDeprecated

- setValueChangeHandlerDeprecated

- setValueChangeHandlerDeprecated

- setValueChangeHandlerDeprecated

- setValueChangeTargetDeprecated

- setWorkLoopDeprecated

- startDeprecated

- stopDeprecated

- updateValueDeprecated

- validateValueDeprecated

### Type Methods

+ addUserClientActionDeprecated

+ detachUserClientsActionDeprecated

+ removeUserClientActionDeprecated

+ setCommandGateUsageDeprecated

+ setValueActionDeprecated

+ withAttributesDeprecated

## Relationships

### Inherits From

- IOService

## See Also

### Interfaces

IOAudioLevelControl

IOAudioSelectorControl

IOAudioToggleControl

IOAudioEngine

Abstract base class for a single audio audio / I/O engine.

IOAudioStream

This class wraps a single sample buffer in an audio driver.

IOAudioPort

Represents a logical or physical port or functional unit in an audio device.

