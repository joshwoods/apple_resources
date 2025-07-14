

- Kernel
- Hardware Families
- Audio
- IOAudioPort
-  deactivateAudioControls 

# deactivateAudioControls

Called to shut down all of the audio controls for this port.

``` source
virtual void deactivateAudioControls(); 
```

## Overview

This will stop all of the audio controls and release them so that the instances may be freed. This is called from the free() method.

## See Also

### Miscellaneous

addAudioControl

Adds a newly created IOAudioControl instance to the port.

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

