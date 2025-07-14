

- Kernel
- Hardware Families
- Audio
- IOAudioPort
-  addAudioControl 

# addAudioControl

Adds a newly created IOAudioControl instance to the port.

``` source
virtual IOReturn addAudioControl(
 IOAudioControl *control); 
```

## Parameters 

`control`  

A newly created IOAudioControl instance that should belong to this port.

## Return Value

Returns true on successfully staring the IOAudioControl.

## Overview

This method is responsible for starting the new IOAudioControl and adding it to the internal audioControls array.

## See Also

### Miscellaneous

deactivateAudioControls

Called to shut down all of the audio controls for this port.

free

Frees all of the resources allocated by the IOAudioPort.

initWithAttributes

Initializes a newly allocated IOAudioPort instance with the given attributes

start

Called to start a newly created IOAudioPort.

stop

Called when the IOAudioDevice is stopping when it is no longer available.

withAttributes

Allocates a new IOAudioPort instance with the given attributes

