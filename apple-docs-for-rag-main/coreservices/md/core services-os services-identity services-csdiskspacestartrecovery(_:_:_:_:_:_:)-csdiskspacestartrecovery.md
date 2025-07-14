

- Core Services
- OS Services
- Identity Services
-  CSDiskSpaceStartRecovery(\_:\_:\_:\_:\_:\_:) 

Function

# CSDiskSpaceStartRecovery(\_:\_:\_:\_:\_:\_:)

macOS 10.7+

``` source
func CSDiskSpaceStartRecovery(
    _ volumeURL: CFURL!,
    _ bytesNeeded: UInt64,
    _ options: CSDiskSpaceRecoveryOptions,
    _ outOperationUUID: UnsafeMutablePointer?>!,
    _ callbackQueue: dispatch_queue_t!,
    _ callback: CSDiskSpaceRecoveryCallback!
)
```

