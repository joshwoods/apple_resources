

- Core Services
- OS Services
- Identity Services
-  CSIdentityCreate(\_:\_:\_:\_:\_:\_:) 

Function

# CSIdentityCreate(\_:\_:\_:\_:\_:\_:)

macOS 10.5+

``` source
func CSIdentityCreate(
    _ allocator: CFAllocator!,
    _ identityClass: CSIdentityClass,
    _ fullName: CFString!,
    _ posixName: CFString!,
    _ flags: CSIdentityFlags,
    _ authority: CSIdentityAuthority!
) -> Unmanaged!
```

