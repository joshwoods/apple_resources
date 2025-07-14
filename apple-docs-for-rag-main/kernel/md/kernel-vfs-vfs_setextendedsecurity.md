

- Kernel
- vfs
-  vfs_setextendedsecurity 

Function

# vfs_setextendedsecurity

Mark a filesystem as supporting security controls beyond POSIX permissions.

macOS 10.4+

``` source
void vfs_setextendedsecurity(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

void.

## Discussion

Specific controls include ACLs, file owner UUIDs, and group UUIDs.

