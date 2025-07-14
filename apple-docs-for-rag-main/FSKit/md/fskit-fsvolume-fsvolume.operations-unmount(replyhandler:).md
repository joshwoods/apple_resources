

- FSKit
- FSVolume
- FSVolume.Operations
-  unmount(replyHandler:) 

Instance Method

# unmount(replyHandler:)

Unmounts this volume.

macOS 15.4+

``` source
func unmount(replyHandler reply: @escaping () -> Void)
```

``` source
func unmount() async
```

**Required**

## Parameters 

`reply`  

A block or closure to indicate success or failure. If unmounting fails, pass an error as the one parameter to the reply handler. If unmounting succeeds, pass `nil`. For an `async` Swift implementation, there’s no reply handler; simply return normally.

## Discussion

Clear and flush all cached state in your implementation of this method.

## See Also

### Mounting and unmounting

func mount(options: FSTaskOptions, replyHandler: ((any Error)?) -> Void)

Mounts this volume, using the specified options.

**Required**

