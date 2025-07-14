

- Kernel
- Hardware Families
- Audio
- IOAudioLevelControl
-  setLinearScale 

# setLinearScale

This function tells CoreAudio if it should apply a curve to the scaler representation of the volume.

``` source
virtual void setLinearScale(
 booluseLinearScale); 
```

## Parameters 

`useLinearScale`  

TRUE instructs CoreAudio to not apply a curve to the scaler representation of the volume, FALSE instructs CoreAudio to apply a curve, which is CoreAudio's default behavior.

## See Also

### Miscellaneous

create

Allocates a new level control with the given attributes

init

Initializes a newly allocated IOAudioLevelControl with the given attributes

setMaxDB

Sets the maximum value in db that the control may have

setMaxValue

Sets the maximum value the control may have

setMinDB

Sets the minimum value in db that the control may have

setMinValue

Sets the minimum value the control may have

