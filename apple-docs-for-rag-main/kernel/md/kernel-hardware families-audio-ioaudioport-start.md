

- Kernel
- Hardware Families
- Audio
- IOAudioPort
-  start 

# start

Called to start a newly created IOAudioPort.

``` source
virtual bool start(
 IOService *provider); 
```

## Parameters 

`provider`  

The IOAudioDevice that owns this port

## Return Value

Returns true on success

## Overview

This is called automatically by IOAudioDevice when attachAudioPort() is called.

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

stop

Called when the IOAudioDevice is stopping when it is no longer available.

withAttributes

Allocates a new IOAudioPort instance with the given attributes

