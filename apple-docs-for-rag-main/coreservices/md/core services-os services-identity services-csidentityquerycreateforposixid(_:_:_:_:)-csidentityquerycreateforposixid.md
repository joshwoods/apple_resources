

- Core Services
- OS Services
- Identity Services
-  CSIdentityQueryCreateForPosixID(\_:\_:\_:\_:) 

Function

# CSIdentityQueryCreateForPosixID(\_:\_:\_:\_:)

macOS 10.5+

``` source
func CSIdentityQueryCreateForPosixID(
    _ allocator: CFAllocator!,
    _ posixID: id_t,
    _ identityClass: CSIdentityClass,
    _ authority: CSIdentityAuthority!
) -> Unmanaged!
```

