

- Foundation
- URLResourceValues
-  volumeIdentifier 

Instance Property

# volumeIdentifier

An identifier that identifies the volume the file system object is on.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var volumeIdentifier: (any NSCopying & NSSecureCoding & NSObjectProtocol)? { get }
```

## Discussion

Other objects on the same volume will have the same volume identifier and can be compared using for equality using `isEqual`. This identifier is not persistent across system restarts.

## See Also

### Volume support values

var isMountTrigger: Bool?

A Boolean value that indicates whether this URL is a file system trigger directory.

var isVolume: Bool?

A Boolean value that indicates whether the root directory is a volume.

var volume: URL?

URL of the volume on which the resource is stored.

var volumeCreationDate: Date?

The volume’s creation date, or `nil` if this cannot be determined.

var volumeLocalizedFormatDescription: String?

The volume format that’s visible to the user.

var volumeLocalizedName: String?

The name of the volume that’s visible to the user.

var volumeMaximumFileSize: Int?

The largest file size supported by this file system, in bytes, or `nil` if this cannot be determined.

var volumeName: String?

The name of the volume.

var volumeResourceCount: Int?

The total number of resources on the volume.

var volumeSupportsAccessPermissions: Bool?

A Boolean value that indicates whether the volume supports setting standard access permissions.

var volumeSupportsAdvisoryFileLocking: Bool?

A Boolean value that indicates whether the volume implements whole-file flock(2) style advisory locks, and the O_EXLOCK and O_SHLOCK flags of the open(2) call.

var volumeSupportsCasePreservedNames: Bool?

A Boolean value that indicates whether the volume format preserves the case of file and directory names.

var volumeSupportsCaseSensitiveNames: Bool?

A Boolean value that indicates whether the volume format treats upper and lower case characters in file and directory names as different.

var volumeSupportsCompression: Bool?

A Boolean value that indicates whether the volume supports transparent decompression of compressed files using decmpfs.

var volumeSupportsExclusiveRenaming: Bool?

A Boolean value that indicates whether the volume warns of a pre-existing destination when renaming a file.

