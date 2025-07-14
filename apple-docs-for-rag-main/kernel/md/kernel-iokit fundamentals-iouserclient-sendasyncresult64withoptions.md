

- Kernel
- IOKit Fundamentals
- IOUserClient
-  sendAsyncResult64WithOptions 

# sendAsyncResult64WithOptions

Send a notification as with sendAsyncResult, but with finite queueing.

``` source
static IOReturn sendAsyncResult64WithOptions(
 OSAsyncReference64 reference, 
 IOReturn result,
 io_user_reference_t args[],
 UInt32 numArgs, 
 IOOptionBits options); 
```

## Overview

IOUserClient::sendAsyncResult64() will infitely queue messages if the client is not processing them in a timely fashion. This variant will not, for simple handling of situations where clients may be expected to stop processing messages.

## See Also

### Miscellaneous

exportObjectToClient

releaseAsyncReference64

Release the mach_port_t reference held within the OSAsyncReference64 structure.

releaseNotificationPort

Release the mach_port_t passed to registerNotificationPort().

removeMappingForDescriptor

