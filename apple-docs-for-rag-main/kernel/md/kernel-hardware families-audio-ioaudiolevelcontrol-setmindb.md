

- Kernel
- Hardware Families
- Audio
- IOAudioLevelControl
-  setMinDB 

# setMinDB

Sets the minimum value in db that the control may have

``` source
virtual void setMinDB(
 IOFixedminDB); 
```

## Parameters 

`minDB`  

The minimum value in db for the control

## Overview

This value is represented as an IOFixed value which is a fixed point number. The IOFixed type is a 16.16 fixed point value.

## See Also

### Miscellaneous

create

Allocates a new level control with the given attributes

init

Initializes a newly allocated IOAudioLevelControl with the given attributes

setLinearScale

This function tells CoreAudio if it should apply a curve to the scaler representation of the volume.

setMaxDB

Sets the maximum value in db that the control may have

setMaxValue

Sets the maximum value the control may have

setMinValue

Sets the minimum value the control may have

