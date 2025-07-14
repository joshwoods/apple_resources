

- Kernel
- Hardware Families
- Audio
- IOAudioLevelControl
-  create 

# create

Allocates a new level control with the given attributes

``` source
static IOAudioLevelControl *create(
 SInt32 initialValue, 
 SInt32 minValue, 
 SInt32 maxValue, 
 IOFixed minDB, 
 IOFixed maxDB, 
 UInt32 channelID, 
 const char *channelName = 0, 
 UInt32 cntrlID = 0, 
 UInt32 subType = 0, 
 UInt32 usage = 0); 
```

## Parameters 

`initialValue`  

The initial value of the control

`minValue`  

The lowest possible value the control may have

`maxValue`  

The highest possible value the control may have

`minDB`  

A fixed point representation of the db value matching minValue

`maxDB`  

A fixed point representation of the db value matching maxValue

`channelID`  

The ID of the channel(s) that the control acts on. Common IDs are located in IOAudioTypes.h.

`channelName`  

An optional name for the channel. Common names are located in IOAudioTypes.h.

`cntrlID`  

An optional ID for the control that can be used to uniquely identify controls.

## Return Value

Returns a newly allocted and initialized level IOAudioControl

## See Also

### Miscellaneous

init

Initializes a newly allocated IOAudioLevelControl with the given attributes

setLinearScale

This function tells CoreAudio if it should apply a curve to the scaler representation of the volume.

setMaxDB

Sets the maximum value in db that the control may have

setMaxValue

Sets the maximum value the control may have

setMinDB

Sets the minimum value in db that the control may have

setMinValue

Sets the minimum value the control may have

