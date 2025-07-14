

- Kernel
- Hardware Families
- Audio
- IOAudioPort
-  stop 

# stop

Called when the IOAudioDevice is stopping when it is no longer available.

``` source
virtual void stop(
 IOService *provider); 
```

## Parameters 

`provider`  

The IOAudioDevice that owns this port

## Overview

This method calls deactivateAudioControls() to shut down all of the controls associated with this port.

## See Also

### Miscellaneous

addAudioControl

Adds a newly created IOAudioControl instance to the port.

deactivateAudioControls

Called to shut down all of the audio controls for this port.

free

Frees all of the resources allocated by the IOAudioPort.

initWithAttributes

Initializes a newly allocated IOAudioPort instance with the given attributes

start

Called to start a newly created IOAudioPort.

withAttributes

Allocates a new IOAudioPort instance with the given attributes

