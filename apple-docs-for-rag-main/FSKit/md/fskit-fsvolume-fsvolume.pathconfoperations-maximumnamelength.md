

- FSKit
- FSVolume
- FSVolume.PathConfOperations
-  maximumNameLength 

Instance Property

# maximumNameLength

A property that represents the maximum length of a component of a filename.

macOS 15.4+

``` source
var maximumNameLength: Int { get }
```

**Required**

## See Also

### Checking limits and configurations

var maximumLinkCount: Int

A property that represents the maximum number of hard links to the object.

**Required**

var restrictsOwnershipChanges: Bool

A Boolean property that indicates whether the volume restricts ownership changes based on authorization.

**Required**

var truncatesLongNames: Bool

A property that indicates whether the volume truncates files longer than its maximum supported length.

**Required**

var maximumFileSize: UInt64

The maximum size of a regular file allowed in the volume.

var maximumFileSizeInBits: Int

The minimum number of bits needed to represent, as a signed integer value, the maximum size of a regular file allowed in the volume.

var maximumXattrSize: Int

The maximum extended attribute size in bytes.

var maximumXattrSizeInBits: Int

The maximum extended attribute size in bits.

