

- Kernel
- vfs
-  vfs_setauthcache_ttl 

Function

# vfs_setauthcache_ttl

Enable credential caching and set time-to-live of cached authorized credentials for files in this filesystem.

macOS 10.5+

``` source
void vfs_setauthcache_ttl(mount_t mp, int ttl);
```

## Parameters 

`mp`  

Mount for which to set cache lifetime.

## Return Value

void.

## Discussion

If a filesystem is set to allow caching credentials, the VFS layer can authorize previously-authorized actions from the same vfs_context_t without calling down to the filesystem (though it will not deny based on the cache).

