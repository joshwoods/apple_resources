

- FSKit
- FSVolume
- FSVolume.Operations
-  synchronize(flags:replyHandler:) 

Instance Method

# synchronize(flags:replyHandler:)

Synchronizes the volume with its underlying resource.

macOS 15.4+

``` source
func synchronize(
    flags: FSSyncFlags,
    replyHandler reply: @escaping ((any Error)?) -> Void
)
```

``` source
func synchronize(flags: FSSyncFlags) async throws
```

**Required**

## Parameters 

`flags`  

Timing flags, as defined in `mount.h.` These flags let the file system know whether to run the operation in a blocking or nonblocking fashion.

`reply`  

A block or closure to indicate success or failure. If synchronization fails, pass an error as the one parameter to the reply handler. If synchronization succeeds, pass `nil`. For an `async` Swift implementation, there’s no reply handler; simply throw an error or return normally.

## Discussion

After calling this method, FSKit assumes that the volume has sent all pending I/O or metadata to its resource.

## See Also

### Synchronizing with a resource

enum FSSyncFlags

Behavior flags for use with synchronization calls.

