

- FSKit
- FSItem
-  FSItem.Attributes 

Class

# FSItem.Attributes

Attributes of an item, such as size, creation and modification times, and user and group identifiers.

macOS 15.4+

``` source
class Attributes
```

## Topics

### Validating and invalidating attributes

func isValid(FSItem.Attribute) -> Bool

Returns a Boolean value that indicates whether the attribute is valid.

func invalidateAllProperties()

Marks all attributes inactive.

### Working with identifier attributes

var fileID: FSItem.Identifier

The item’s file identifier.

var parentID: FSItem.Identifier

The identifier of the item’s parent.

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

var inhibitKernelOffloadedIO: Bool

A Boolean value that indicates whether the file system overrides the per-volume settings for kernel offloaded I/O for a specific file.

### Working with time attributes

var accessTime: timespec

The item’s last-accessed time.

var modifyTime: timespec

The item’s last-modified time.

var changeTime: timespec

The item’s last-changed time.

var birthTime: timespec

The item’s creation time.

var backupTime: timespec

The item’s last-backup time.

var addedTime: timespec

The item’s added time.

## Relationships

### Inherits From

- NSObject

### Inherited By

- FSItem.SetAttributesRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Working with attributes

class GetAttributesRequest

A request to get attributes from an item.

class SetAttributesRequest

A request to set attributes on an item.

