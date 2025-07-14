

- Kernel
- IOKit Fundamentals
- IOUserClient
-  releaseAsyncReference64 

# releaseAsyncReference64

Release the mach_port_t reference held within the OSAsyncReference64 structure.

``` source
static IOReturn releaseAsyncReference64(
 OSAsyncReference64reference); 
```

## Parameters 

`reference`  

The reference passed to the subclass IOAsyncMethod, or externalMethod() in the IOExternalMethodArguments.asyncReference field.

## Return Value

A return code.

## Overview

The OSAsyncReference64 structure passed to async methods holds a reference to the wakeup mach port, which should be released to balance each async method call. Behavior is undefined if these calls are not correctly balanced.

## See Also

### Miscellaneous

exportObjectToClient

releaseNotificationPort

Release the mach_port_t passed to registerNotificationPort().

removeMappingForDescriptor

sendAsyncResult64WithOptions

Send a notification as with sendAsyncResult, but with finite queueing.

