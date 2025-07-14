

- Core Services
- OS Services
- Identity Services
-  CSIdentityQueryCreateForName(\_:\_:\_:\_:\_:) 

Function

# CSIdentityQueryCreateForName(\_:\_:\_:\_:\_:)

Mac Catalyst 13.1+macOS 10.5+

``` source
func CSIdentityQueryCreateForName(
    _ allocator: CFAllocator!,
    _ name: CFString!,
    _ comparisonMethod: CSIdentityQueryStringComparisonMethod,
    _ identityClass: CSIdentityClass,
    _ authority: CSIdentityAuthority!
) -> Unmanaged!
```

