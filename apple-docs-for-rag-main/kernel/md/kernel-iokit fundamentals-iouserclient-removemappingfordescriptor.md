

- Kernel
- IOKit Fundamentals
- IOUserClient
-  removeMappingForDescriptor 

# removeMappingForDescriptor

``` source
IOMemoryMap * removeMappingForDescriptor(
 IOMemoryDescriptor *memory); 
```

## Parameters 

`memory`  

The memory descriptor instance previously returned by the implementation of clientMemoryForType().

## Return Value

A reference to the first IOMemoryMap instance found in the list of mappings created by IOUserClient from that passed memory descriptor is returned, or zero if none exist. The caller should release this reference.

## Overview

Remove the first mapping created from the memory descriptor returned by clientMemoryForType() from IOUserClient's list of mappings. If such a mapping exists, it is retained and the reference currently held by IOUserClient is returned to the caller.

## See Also

### Miscellaneous

exportObjectToClient

releaseAsyncReference64

Release the mach_port_t reference held within the OSAsyncReference64 structure.

releaseNotificationPort

Release the mach_port_t passed to registerNotificationPort().

sendAsyncResult64WithOptions

Send a notification as with sendAsyncResult, but with finite queueing.

