

- FSKit
- FSItem
- FSItem.Attributes
-  gid 

Instance Property

# gid

The group identifier.

macOS 15.4+

``` source
var gid: UInt32 { get set }
```

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

var flags: UInt32

The item’s behavior flags.

var size: UInt64

The item’s size.

var allocSize: UInt64

The item’s allocated size.

var supportsLimitedXAttrs: Bool

A Boolean value that indicates whether the item supports a limited set of extended attributes.

var inhibitKernelOffloadedIO: Bool

A Boolean value that indicates whether the file system overrides the per-volume settings for kernel offloaded I/O for a specific file.

