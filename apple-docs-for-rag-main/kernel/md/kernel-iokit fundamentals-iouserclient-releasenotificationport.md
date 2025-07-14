

- Kernel
- IOKit Fundamentals
- IOUserClient
-  releaseNotificationPort 

# releaseNotificationPort

Release the mach_port_t passed to registerNotificationPort().

``` source
static IOReturn releaseNotificationPort(
 mach_port_treference); 
```

## Parameters 

`reference`  

The mach_port_t argument previously passed to the subclass implementation of registerNotificationPort().

## Return Value

A return code.

## Overview

The mach_port_t passed to the registerNotificationPort() methods should be released to balance each call to registerNotificationPort(). Behavior is undefined if these calls are not correctly balanced.

## See Also

### Miscellaneous

exportObjectToClient

releaseAsyncReference64

Release the mach_port_t reference held within the OSAsyncReference64 structure.

removeMappingForDescriptor

sendAsyncResult64WithOptions

Send a notification as with sendAsyncResult, but with finite queueing.

