

- Foundation
- URLResourceKey
-  volumeSupportsRootDirectoryDatesKey 

Type Property

# volumeSupportsRootDirectoryDatesKey

Key for determining whether the volume supports reliable storage of times for the root directory, returned as a Boolean `NSNumber` object (read-only).

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let volumeSupportsRootDirectoryDatesKey: URLResourceKey
```

## See Also

### Volume support keys

static let isMountTriggerKey: URLResourceKey

Key for determining whether the URL is a file system trigger directory, returned as a Boolean `NSNumber` object (read-only). Traversing or opening a file system trigger directory causes an attempt to mount a file system on the directory.

static let isVolumeKey: URLResourceKey

Key for determining whether the resource is the root directory of a volume, returned as a Boolean `NSNumber` object (read-only).

static let volumeCreationDateKey: URLResourceKey

Key for the volume’s creation date, returned as an `NSDate` object, or `NULL` if it cannot be determined (read-only).

static let volumeIdentifierKey: URLResourceKey

The unique identifier of the resource’s volume, returned as an `id` (read-only).

static let volumeLocalizedFormatDescriptionKey: URLResourceKey

Key for the volume’s descriptive format name, returned as an `NSString` object (read-only).

static let volumeLocalizedNameKey: URLResourceKey

The name of the volume as it should be displayed in the user interface, returned as an `NSString` object (read-only).

static let volumeMaximumFileSizeKey: URLResourceKey

Key for the largest file size supported by the volume in bytes, returned as a Boolean `NSNumber` object, or `nil` if it cannot be determined (read-only).

static let volumeNameKey: URLResourceKey

The name of the volume, returned as an `NSString` object (read-write). Settable only if `NSURLVolumeSupportsRenamingKey` is true.

static let volumeResourceCountKey: URLResourceKey

Key for the total number of resources on the volume, returned as an `NSNumber` object (read-only).

static let volumeSupportsAccessPermissionsKey: URLResourceKey

static let volumeSupportsAdvisoryFileLockingKey: URLResourceKey

Key for determining whether the volume implements whole-file advisory locks in the style of flock, along with the `O_EXLOCK` and `O_SHLOCK` flags of the open function, returned as a Boolean `NSNumber` object (read-only).

static let volumeSupportsCasePreservedNamesKey: URLResourceKey

Key for determining whether the volume supports case-preserved names, returned as a Boolean `NSNumber` object (read-only).

static let volumeSupportsCaseSensitiveNamesKey: URLResourceKey

Key for determining whether the volume supports case-sensitive names, returned as a Boolean `NSNumber` object (read-only).

static let volumeSupportsCompressionKey: URLResourceKey

Whether the volume supports transparent decompression of compressed files using `decmpfs`, returned as `NSNumber` containing a Boolean value (read-only).

static let volumeSupportsExclusiveRenamingKey: URLResourceKey

Whether the volume supports exclusive renaming using `renamex_np(2)` with the `RENAME_EXCL` option, returned as `NSNumber` containing a Boolean value (read-only).

