

- Kernel
- vfs
-  vfs_authcache_ttl 

Function

# vfs_authcache_ttl

Determine the time-to-live of cached authorized credentials for files in this filesystem.

macOS 10.5+

``` source
int vfs_authcache_ttl(mount_t mp);
```

## Parameters 

`mp`  

Mount for which to check cache lifetime.

## Return Value

Cache lifetime in seconds. CACHED_RIGHT_INFINITE_TTL indicates that credentials never expire.

## Discussion

If a filesystem is set to allow caching credentials, the VFS layer can authorize previously-authorized actions from the same vfs_context_t without calling down to the filesystem (though it will not deny based on the cache).

