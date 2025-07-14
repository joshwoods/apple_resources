

- Kernel
- Hardware Families
- Audio
- IOAudioToggleControl
-  create 

# create

Allocates a new mute control with the given attributes

``` source
static IOAudioToggleControl *create(
 bool initialValue, 
 UInt32 channelID, 
 const char *channelName = 0, 
 UInt32 cntrlID = 0, 
 UInt32 subType = 0, 
 UInt32 usage = 0); 
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

createPassThruMuteControl

Allocates a new pass through mute control with the given attributes

init

Initializes a newly allocated IOAudioToggleControl with the given attributes

