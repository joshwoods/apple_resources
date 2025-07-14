

- Kernel
- Hardware Families
- Audio
- IOAudioToggleControl
-  createPassThruMuteControl 

# createPassThruMuteControl

Allocates a new pass through mute control with the given attributes

``` source
static IOAudioToggleControl *createPassThruMuteControl (
 boolinitialValue, 
 UInt32channelID, 
 const char *channelName, 
 UInt32cntrlID); 
```

## Parameters 

`initialValue`  

The initial value of the control

`channelID`  

The ID of the channel(s) that the control acts on. Common IDs are located in IOAudioTypes.h.

`channelName`  

An optional name for the channel. Common names are located in IOAudioPort.h.

`cntrlID`  

An optional ID for the control that can be used to uniquely identify controls

## Return Value

Returns a newly allocated and initialized mute IOAudioControl

## See Also

### Miscellaneous

create

Allocates a new mute control with the given attributes

init

Initializes a newly allocated IOAudioToggleControl with the given attributes

