

- Kernel
- IOKit Fundamentals
- IOUserClient
-  exportObjectToClient 

# exportObjectToClient

``` source
virtual IOReturn exportObjectToClient(
 task_ttask, 
 OSObject *obj,
 io_object_t *clientObj); 
```

## Parameters 

`task`  

The task.

`obj`  

The object we want to export to the client.

`clientObj`  

Returned value is the client's port name.

## Overview

Make an arbitrary OSObject available to the client task.

## See Also

### Miscellaneous

releaseAsyncReference64

Release the mach_port_t reference held within the OSAsyncReference64 structure.

releaseNotificationPort

Release the mach_port_t passed to registerNotificationPort().

removeMappingForDescriptor

sendAsyncResult64WithOptions

Send a notification as with sendAsyncResult, but with finite queueing.

