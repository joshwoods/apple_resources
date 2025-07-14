

- Core Services
- OS Services
- Identity Services
-  CSIdentityQueryCreateForUUID(\_:\_:\_:) 

Function

# CSIdentityQueryCreateForUUID(\_:\_:\_:)

macOS 10.5+

``` source
func CSIdentityQueryCreateForUUID(
    _ allocator: CFAllocator!,
    _ uuid: CFUUID!,
    _ authority: CSIdentityAuthority!
) -> Unmanaged!
```

