

- Foundation
- FileManager
- FileManager.UnmountOptions
-  init(rawValue:) 

Initializer

# init(rawValue:)

macOS 10.11+

``` source
init(rawValue: UInt)
```

## See Also

### Unmount Behavior

static var allPartitionsAndEjectDisk: FileManager.UnmountOptions

Specifies that all partitions on an unmountable disk should be unmounted.

static var withoutUI: FileManager.UnmountOptions

Specifies that no UI should accompany the unmount operation.

