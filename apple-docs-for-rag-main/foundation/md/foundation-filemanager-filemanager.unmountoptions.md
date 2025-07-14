

- Foundation
- FileManager
-  FileManager.UnmountOptions 

Structure

# FileManager.UnmountOptions

Options that specify the behavior of an unmount operation.

macOS 10.11+

``` source
struct UnmountOptions
```

## Topics

### Unmount Behavior

init(rawValue: UInt)

static var allPartitionsAndEjectDisk: FileManager.UnmountOptions

Specifies that all partitions on an unmountable disk should be unmounted.

static var withoutUI: FileManager.UnmountOptions

Specifies that no UI should accompany the unmount operation.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Unmounting Volumes

func unmountVolume(at: URL, options: FileManager.UnmountOptions, completionHandler: ((any Error)?) -> Void)

Starts the process of unmounting the specified volume.

let NSFileManagerUnmountDissentingProcessIdentifierErrorKey: String

The process identifier of the process that prevented a volume from unmounting.

