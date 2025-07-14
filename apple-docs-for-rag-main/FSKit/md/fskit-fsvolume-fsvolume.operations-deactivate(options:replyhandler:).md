

- FSKit
- FSVolume
- FSVolume.Operations
-  deactivate(options:replyHandler:) 

Instance Method

# deactivate(options:replyHandler:)

Tears down a previously initialized volume instance.

macOS 15.4+

``` source
func deactivate(
    options: FSDeactivateOptions = [],
    replyHandler reply: @escaping ((any Error)?) -> Void
)
```

``` source
func deactivate(options: FSDeactivateOptions = []) async throws
```

**Required**

## Parameters 

`options`  

Options to apply to the deactivation.

`reply`  

A block or closure to indicate success or failure. If activation fails, pass an error as the one parameter to the reply handler. If activation succeeds, pass `nil`. For an `async` Swift implementation, there’s no reply handler; simply throw an error or return normally.

## Discussion

Set up your implementation to release any resources allocated for the volume instance. By the time you receive this callback, FSKit has already performed a reclaim call to release all other file nodes associated with this file system instance.

Avoid performing any I/O in this method. Prior to calling this method, FSKit has already issued a sync call to perform any cleanup-related I/O.

FSKit unmounts any mounted volume with a call to unmount(replyHandler:) prior to the deactivate callback.

## See Also

### Handling activation and deactivation

func activate(options: FSTaskOptions, replyHandler: (FSItem?, (any Error)?) -> Void)

Activates the volume using the specified options.

**Required**

class FSItem

A distinct object in a file hierarchy, such as a file, directory, symlink, socket, and more.

struct FSDeactivateOptions

Options that affect the behavior of deactivate methods.

