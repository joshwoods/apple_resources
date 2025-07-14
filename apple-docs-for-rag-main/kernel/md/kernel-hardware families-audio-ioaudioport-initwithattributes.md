

- Kernel
- Hardware Families
- Audio
- IOAudioPort
-  initWithAttributes 

# initWithAttributes

Initializes a newly allocated IOAudioPort instance with the given attributes

``` source
virtual bool initWithAttributes(
 UInt32 portType,
 const char *portName = 0,
 UInt32 subType = 0,
 OSDictionary *properties = 0); 
```

## Parameters 

`portType`  

A readable string representing the type of port. Common port types are defined in IOAudioTypes.h and are prefixed with 'kIOAudioPortType'. Please provide feedback if there are other common port types that should be included.

`portName`  

A readable string representing the name of the port. For example: 'Internal Speaker', 'Line Out'. This field is optional, but useful for providing information to the application/user.

`subType`  

Developer defined readable string representing a subtype for the port. (optional)

`properties`  

Standard property list passed to the init of any new IOService. This dictionary gets stored in the registry for this instance. (optional)

## Return Value

Returns true on success.

## Overview

The properties parameter is passed on the superclass' init(). The portType, subType and properties parameters are optional, however portType is recommended.

## See Also

### Miscellaneous

addAudioControl

Adds a newly created IOAudioControl instance to the port.

deactivateAudioControls

Called to shut down all of the audio controls for this port.

free

Frees all of the resources allocated by the IOAudioPort.

start

Called to start a newly created IOAudioPort.

stop

Called when the IOAudioDevice is stopping when it is no longer available.

withAttributes

Allocates a new IOAudioPort instance with the given attributes

