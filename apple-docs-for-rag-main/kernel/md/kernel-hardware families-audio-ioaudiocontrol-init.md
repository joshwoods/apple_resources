

- Kernel
- Hardware Families
- Audio
- IOAudioControl
-  init 

# init

Initializes a newly allocated IOAudioControl with the given attributes.

``` source
virtual bool init(
 UInt32 type, 
 OSObject *initialValue, 
 UInt32 channelID, 
 const char *channelName = 0, 
 UInt32 cntrlID = 0, 
 UInt32 subType = 0, 
 UInt32 usage = 0, 
 OSDictionary *properties = 0); 
```

## Parameters 

`type`  

The type of the control. Common, known types are defined in IOAudioTypes.h. They currently consist of kIOAudioControlTypeLevel, kIOAudioControlTypeToggle, kIOAudioControlTypeSelector.

`channelID`  

The ID of the channel(s) that the control acts on. Common IDs are located in IOAudioTypes.h.

`channelName`  

An optional name for the channel. Common names are located in IOAudioDefines.h. Any name not defined in IOAudioDefines.h must be localized in order to be properly displayed in multiple languages.

`cntrlID`  

An optional ID for the control that can be used to uniquely identify controls

`subType`  

An optional subType specific to the given type

`usage`  

An optional value specifying how the control will be used. Currently defined usages are kIOAudioControlUsageInput, kIOAudioControlUsageOutput and kIOAudioControlUsagePassThru. This value is used when a control is set as a default control on an IOAudioEngine.

`properties`  

Standard property list passed to the init() function of any new IOService. This dictionary gets stored in the registry entry for this instance.

## Return Value

Returns true on success.

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

