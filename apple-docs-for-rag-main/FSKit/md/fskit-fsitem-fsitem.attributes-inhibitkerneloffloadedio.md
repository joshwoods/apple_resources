

- FSKit
- FSItem
- FSItem.Attributes
-  inhibitKernelOffloadedIO 

Instance Property

# inhibitKernelOffloadedIO

A Boolean value that indicates whether the file system overrides the per-volume settings for kernel offloaded I/O for a specific file.

macOS 15.4+

``` source
var inhibitKernelOffloadedIO: Bool { get set }
```

## Discussion

This property has no meaning if the volume doesn’t conform to FSVolumeKernelOffloadedIOOperations.

## See Also

### Working with metadata attributes

var type: FSItem.ItemType

The item type, such as a regular file, directory, or symbolic link.

var mode: UInt32

The mode of the item.

var linkCount: UInt32

The number of hard links to the item.

var uid: UInt32

The user identifier.

var gid: UInt32

The group identifier.

var flags: UInt32

The item’s behavior flags.

var size: UInt64

The item’s size.

var allocSize: UInt64

The item’s allocated size.

var supportsLimitedXAttrs: Bool

A Boolean value that indicates whether the item supports a limited set of extended attributes.

