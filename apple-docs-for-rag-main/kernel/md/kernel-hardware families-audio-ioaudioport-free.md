

- Kernel
- Hardware Families
- Audio
- IOAudioPort
-  free 

# free

Frees all of the resources allocated by the IOAudioPort.

``` source
virtual void free(); 
```

## Overview

Do not call this directly. This is called automatically by the system when the instance's refcount goes to 0. To decrement the refcount, call release() on the object.

## See Also

### Miscellaneous

addAudioControl

Adds a newly created IOAudioControl instance to the port.

deactivateAudioControls

Called to shut down all of the audio controls for this port.

initWithAttributes

Initializes a newly allocated IOAudioPort instance with the given attributes

start

Called to start a newly created IOAudioPort.

stop

Called when the IOAudioDevice is stopping when it is no longer available.

withAttributes

Allocates a new IOAudioPort instance with the given attributes

