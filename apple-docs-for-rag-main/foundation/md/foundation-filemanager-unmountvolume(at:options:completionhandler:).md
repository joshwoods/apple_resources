

- Foundation
- FileManager
-  unmountVolume(at:options:completionHandler:) 

Instance Method

# unmountVolume(at:options:completionHandler:)

Starts the process of unmounting the specified volume.

macOS 10.11+

``` source
func unmountVolume(
    at url: URL,
    options mask: FileManager.UnmountOptions = [],
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func unmountVolume(
    at url: URL,
    options mask: FileManager.UnmountOptions = []
) async throws
```

## Parameters 

`url`  

A file URL specifying the volume to be unmounted.

`mask`  

A bitmask of FileManager.UnmountOptions that you can use to customize the unmount operation’s behavior.

`completionHandler`  

A block executed when the unmount operation completes. The block receives an error parameter which is `nil` if unmounting was successful. Otherwise, it indicates why unmounting failed.

## Discussion

If the volume is encrypted, it is relocked after being unmounted.

## See Also

### Unmounting Volumes

struct UnmountOptions

Options that specify the behavior of an unmount operation.

let NSFileManagerUnmountDissentingProcessIdentifierErrorKey: String

The process identifier of the process that prevented a volume from unmounting.

