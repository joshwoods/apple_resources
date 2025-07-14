

- Core Services
- OS Services
- Identity Services
-  CSIdentityCommitAsynchronously(\_:\_:\_:\_:\_:) 

Function

# CSIdentityCommitAsynchronously(\_:\_:\_:\_:\_:)

macOS 10.5+

``` source
func CSIdentityCommitAsynchronously(
    _ identity: CSIdentity!,
    _ clientContext: UnsafePointer!,
    _ runLoop: CFRunLoop!,
    _ runLoopMode: CFString!,
    _ authorization: AuthorizationRef!
) -> Bool
```

