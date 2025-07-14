

- Kernel
- vfs
-  vfs_clearauthcache_ttl 

Function

# vfs_clearauthcache_ttl

Remove time-to-live controls for cached credentials on a filesytem. Filesystems with remote authorization decisions (opaque) will still have KAUTH_VNODE_SEARCH rights cached for a default of CACHED_LOOKUP_RIGHT_TTL seconds.

macOS 10.5+

``` source
void vfs_clearauthcache_ttl(mount_t mp);
```

## Parameters 

`mp`  

Mount for which to clear cache lifetime.

## Return Value

void.

