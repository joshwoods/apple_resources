

- FSKit
- FSVolume
- FSVolume.PathConfOperations
-  maximumFileSizeInBits 

Instance Property

# maximumFileSizeInBits

The minimum number of bits needed to represent, as a signed integer value, the maximum size of a regular file allowed in the volume.

macOS 15.4+

``` source
optional var maximumFileSizeInBits: Int { get }
```

## Discussion

The maximum file size is `2^(maximumFileSizeInBits - 1)`.

| Maximum file size (bytes)  | Maximum (in hex)     | Unsigned bits | Signed bits |
|----------------------------|----------------------|---------------|-------------|
| 65,535                     | `0xFFFF`             | 16            | 17          |
| 2,147,483,647              | `0x7FFFFFFF`         | 31            | 32          |
| 4,294,967,295              | `0xFFFFFFFF`         | 32            | 33          |
| 18,446,744,073,709,551,615 | `0xFFFFFFFFFFFFFFFF` | 64            | 65          |

Implement at least one of maximumFileSize or `maximumFileSizeInBits`. FSKit automatically converts from one to another if needed. If you implement both, FSKit uses only the `maximumFileSizeInBits` implementation.

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

var truncatesLongNames: Bool

A property that indicates whether the volume truncates files longer than its maximum supported length.

**Required**

var maximumFileSize: UInt64

The maximum size of a regular file allowed in the volume.

var maximumXattrSize: Int

The maximum extended attribute size in bytes.

var maximumXattrSizeInBits: Int

The maximum extended attribute size in bits.

