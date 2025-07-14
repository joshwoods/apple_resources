

- Foundation
- FileManager
- FileManager.UnmountOptions
-  withoutUI 

Type Property

# withoutUI

Specifies that no UI should accompany the unmount operation.

macOS 10.11+

``` source
static var withoutUI: FileManager.UnmountOptions { get }
```

## Discussion

If this option is not specified when calling unmountVolume(at:options:completionHandler:), any needed UI will delay completion of the completion handler.

## See Also

### Unmount Behavior

init(rawValue: UInt)

static var allPartitionsAndEjectDisk: FileManager.UnmountOptions

Specifies that all partitions on an unmountable disk should be unmounted.

