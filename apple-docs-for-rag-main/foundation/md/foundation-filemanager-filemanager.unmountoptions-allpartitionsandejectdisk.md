

- Foundation
- FileManager
- FileManager.UnmountOptions
-  allPartitionsAndEjectDisk 

Type Property

# allPartitionsAndEjectDisk

Specifies that all partitions on an unmountable disk should be unmounted.

macOS 10.11+

``` source
static var allPartitionsAndEjectDisk: FileManager.UnmountOptions { get }
```

## Discussion

If the volume is on a partitioned disk, this option unmounts all volumes on that disk. Then, then the disk is ejected (if it is ejectable).

## See Also

### Unmount Behavior

init(rawValue: UInt)

static var withoutUI: FileManager.UnmountOptions

Specifies that no UI should accompany the unmount operation.

