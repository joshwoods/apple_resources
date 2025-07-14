

- FSKit
- FSVolume
- FSVolume.Operations
-  mount(options:replyHandler:) 

Instance Method

# mount(options:replyHandler:)

Mounts this volume, using the specified options.

macOS 15.4+

``` source
func mount(
    options: FSTaskOptions,
    replyHandler reply: @escaping ((any Error)?) -> Void
)
```

``` source
func mount(options: FSTaskOptions) async throws
```

**Required**

## Parameters 

`options`  

Options to apply to the mount. These can include security-scoped file paths. There are no defined options currently.

`reply`  

A block or closure to indicate success or failure. If mounting fails, pass an error as the one parameter to the reply handler. If mounting succeeds, pass `nil`. For an `async` Swift implementation, there’s no reply handler; simply return normally.

## Discussion

FSKit calls this method as a signal that some process is trying to mount this volume. Your file system receives a call to activate(options:replyHandler:) prior to receiving any mount calls.

## See Also

### Mounting and unmounting

func unmount(replyHandler: () -> Void)

Unmounts this volume.

**Required**

