

- Core Services
- OS Services
- Identity Services
-  CSIdentityQueryExecuteAsynchronously(\_:\_:\_:\_:\_:) 

Function

# CSIdentityQueryExecuteAsynchronously(\_:\_:\_:\_:\_:)

Mac Catalyst 13.1+macOS 10.5+

``` source
func CSIdentityQueryExecuteAsynchronously(
    _ query: CSIdentityQuery!,
    _ flags: CSIdentityQueryFlags,
    _ clientContext: UnsafePointer!,
    _ runLoop: CFRunLoop!,
    _ runLoopMode: CFString!
) -> Bool
```

