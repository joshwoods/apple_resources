

- Foundation
-  NSFileManagerUnmountDissentingProcessIdentifierErrorKey 

Global Variable

# NSFileManagerUnmountDissentingProcessIdentifierErrorKey

The process identifier of the process that prevented a volume from unmounting.

macOS 10.11+

``` source
let NSFileManagerUnmountDissentingProcessIdentifierErrorKey: String
```

## Discussion

If unmountVolume(at:options:completionHandler:) fails, the error sent to its completion handler will contain a `userInfo` dictionary with this string as one of its keys. The value is the process identifier of the process that prevented the unmounting, as an NSNumber.

## See Also

### Unmounting Volumes

func unmountVolume(at: URL, options: FileManager.UnmountOptions, completionHandler: ((any Error)?) -> Void)

Starts the process of unmounting the specified volume.

struct UnmountOptions

Options that specify the behavior of an unmount operation.

