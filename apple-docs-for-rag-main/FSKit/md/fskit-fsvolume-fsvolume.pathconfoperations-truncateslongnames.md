

- FSKit
- FSVolume
- FSVolume.PathConfOperations
-  truncatesLongNames 

Instance Property

# truncatesLongNames

A property that indicates whether the volume truncates files longer than its maximum supported length.

macOS 15.4+

``` source
var truncatesLongNames: Bool { get }
```

**Required**

## Discussion

If this value is `true`, the volume truncates the filename to maximumNameLength if the filename is longer than that. If this value is false, the file system responds with the error code `ENAMETOOLONG` if the filename is longer than maximumNameLength.

## See Also

### Checking limits and configurations

var maximumLinkCount: Int

A property that represents the maximum number of hard links to the object.

**Required**

var maximumNameLength: Int

A property that represents the maximum length of a component of a filename.

**Required**

var restrictsOwnershipChanges: Bool

A Boolean property that indicates whether the volume restricts ownership changes based on authorization.

**Required**

var maximumFileSize: UInt64

The maximum size of a regular file allowed in the volume.

var maximumFileSizeInBits: Int

The minimum number of bits needed to represent, as a signed integer value, the maximum size of a regular file allowed in the volume.

var maximumXattrSize: Int

The maximum extended attribute size in bytes.

var maximumXattrSizeInBits: Int

The maximum extended attribute size in bits.

