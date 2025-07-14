

- Kernel
- vfs
-  vfs_clearextendedsecurity 

Function

# vfs_clearextendedsecurity

Mark a filesystem as NOT supporting security controls beyond POSIX permissions.

macOS 10.4+

``` source
void vfs_clearextendedsecurity(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

void.

## Discussion

Specific controls include ACLs, file owner UUIDs, and group UUIDs.

