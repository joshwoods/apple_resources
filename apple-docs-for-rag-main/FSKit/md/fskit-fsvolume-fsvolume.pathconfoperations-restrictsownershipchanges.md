

- FSKit
- FSVolume
- FSVolume.PathConfOperations
-  restrictsOwnershipChanges 

Instance Property

# restrictsOwnershipChanges

A Boolean property that indicates whether the volume restricts ownership changes based on authorization.

macOS 15.4+

``` source
var restrictsOwnershipChanges: Bool { get }
```

**Required**

## Discussion

If this value is true, the volume rejects a `chown(2)` from anyone other than the superuser.

## See Also

### Checking limits and configurations

var maximumLinkCount: Int

A property that represents the maximum number of hard links to the object.

**Required**

var maximumNameLength: Int

A property that represents the maximum length of a component of a filename.

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

