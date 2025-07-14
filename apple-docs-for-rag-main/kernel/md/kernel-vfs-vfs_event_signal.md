

- Kernel
- vfs
-  vfs_event_signal 

Function

# vfs_event_signal

Post a kqueue-style event on a filesystem (EVFILT_FS).

macOS 10.4+

``` source
void vfs_event_signal(fsid_t *fsid, u_int32_t event, intptr_t data);
```

## Parameters 

`fsid`  

Unused.

`event`  

Events to post.

`data`  

Unused.

## Return Value

void.

