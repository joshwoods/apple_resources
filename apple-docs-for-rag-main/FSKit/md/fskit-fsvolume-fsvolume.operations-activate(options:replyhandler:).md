

- FSKit
- FSVolume
- FSVolume.Operations
-  activate(options:replyHandler:) 

Instance Method

# activate(options:replyHandler:)

Activates the volume using the specified options.

macOS 15.4+

``` source
func activate(
    options: FSTaskOptions,
    replyHandler reply: @escaping (FSItem?, (any Error)?) -> Void
)
```

``` source
func activate(options: FSTaskOptions) async throws -> FSItem
```

**Required**

## Parameters 

`options`  

Options to apply to the activation. These can include security-scoped file paths. There are no defined options currently.

`reply`  

A block or closure to indicate success or failure. If activation succeeds, pass the root FSItem and a `nil` error. If activation fails, pass the relevant error as the second parameter; FSKit ignores any FSItem in this case. In Swift, `reply` takes only the FSItem as the parameter; you signal any error with a `throw`. For an `async` Swift implementation, there’s no reply handler; simply return the FSItem or throw an error.

## Discussion

When FSKit calls this method, allocate any in-memory state required to represent the file system. Also allocate an FSItem for the root directory of the file system, and pass it to the reply block. FSKit caches this root item for the lifetime of the volume, and uses it as a starting point for all file look-ups.

Volume activation occurs prior to any call to mount the volume.

## See Also

### Handling activation and deactivation

class FSItem

A distinct object in a file hierarchy, such as a file, directory, symlink, socket, and more.

func deactivate(options: FSDeactivateOptions, replyHandler: ((any Error)?) -> Void)

Tears down a previously initialized volume instance.

**Required**

struct FSDeactivateOptions

Options that affect the behavior of deactivate methods.

