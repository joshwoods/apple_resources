

- Foundation
-  URLResourceKey 

Structure

# URLResourceKey

Keys that apply to file system URLs.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct URLResourceKey
```

## Discussion

To request information using one of these keys, pass it to the `forKey:` parameter of the getResourceValue(_:forKey:) instance method.

## Topics

### Application keys

static let isApplicationKey: URLResourceKey

static let applicationIsScriptableKey: URLResourceKey

### Directory keys

static let isDirectoryKey: URLResourceKey

A key for determining whether the resource is a directory.

static let parentDirectoryURLKey: URLResourceKey

The container directory of the resource.

static let directoryEntryCountKey: URLResourceKey

The key for a count of items in the directory.

### File keys

static let fileAllocatedSizeKey: URLResourceKey

The key for the total allocated size on-disk for the file.

static let fileProtectionKey: URLResourceKey

The key for the protection level of the file.

struct URLFileProtection

Protection-level values for a URL resource key.

static let fileContentIdentifierKey: URLResourceKey

The key for a value that APFS assigns to identify a file’s content data stream.

static let fileResourceIdentifierKey: URLResourceKey

The key for the resource’s unique identifier.

static let fileResourceTypeKey: URLResourceKey

The key for the resource’s object type.

struct URLFileResourceType

Possible values for the type of file resource.

static let fileSecurityKey: URLResourceKey

The key for the resource’s security information.

static let fileSizeKey: URLResourceKey

The key for the file’s size, in bytes.

static let isAliasFileKey: URLResourceKey

The key for determining whether the file is an alias.

static let isPackageKey: URLResourceKey

The key for determining whether the resource is a file package.

static let isRegularFileKey: URLResourceKey

The key for determining whether the resource is a regular file rather than a directory or a symbolic link.

static let isPurgeableKey: URLResourceKey

The key for a Boolean value that indicates whether the file system can delete a file when the system needs to free space.

static let isSparseKey: URLResourceKey

The key for a Boolean value that indicates whether the file has sparse regions.

static let mayHaveExtendedAttributesKey: URLResourceKey

The key for a Boolean value that indicates whether the file has extended attributes.

static let mayShareFileContentKey: URLResourceKey

The key for a Boolean value that indicates whether cloned files and their original files may share data blocks.

static let preferredIOBlockSizeKey: URLResourceKey

The key for the optimal block size to use when reading or writing the file’s data.

static let totalFileAllocatedSizeKey: URLResourceKey

The key for the total allocated size of the file, in bytes.

static let totalFileSizeKey: URLResourceKey

The key for the total displayable size of the file, in bytes.

static let fileIdentifierKey: URLResourceKey

The key for the file system’s internal inode identifier for the item.

### Volume capacity keys

Checking Volume Storage Capacity

Confirm that you have enough local storage space for a large amount of data.

static let volumeAvailableCapacityKey: URLResourceKey

Key for the volume’s available capacity in bytes (read-only).

static let volumeAvailableCapacityForImportantUsageKey: URLResourceKey

Key for the volume’s available capacity in bytes for storing important resources (read-only).

static let volumeAvailableCapacityForOpportunisticUsageKey: URLResourceKey

Key for the volume’s available capacity in bytes for storing nonessential resources (read-only).

static let volumeTotalCapacityKey: URLResourceKey

Key for the volume’s total capacity in bytes (read-only).

### Volume status keys

static let volumeIsAutomountedKey: URLResourceKey

A key for determining whether the volume is automounted.

static let volumeIsBrowsableKey: URLResourceKey

A key for determining whether the volume is visible in GUI-based file-browsing environments, such as the Desktop or the Finder app.

static let volumeIsEjectableKey: URLResourceKey

A key for determining whether the volume is ejectable from the drive mechanism under software control.

static let volumeIsEncryptedKey: URLResourceKey

A key for determining whether the volume is encrypted.

static let volumeIsInternalKey: URLResourceKey

A key for determining whether the volume is connected to an internal bus.

static let volumeIsJournalingKey: URLResourceKey

A key for determining whether the volume is currently journaling.

static let volumeIsLocalKey: URLResourceKey

A key for determining whether the volume is on a local device.

static let volumeIsReadOnlyKey: URLResourceKey

A key for determining whether the volume is read-only.

static let volumeIsRemovableKey: URLResourceKey

A key for determining whether the volume is removable from the drive mechanism.

static let volumeIsRootFileSystemKey: URLResourceKey

A key for determining whether the volume is the root file system.

static let volumeSupportsFileProtectionKey: URLResourceKey

A Boolean value that indicates the volume supports data protection for files.

static let volumeTypeNameKey: URLResourceKey

The key for the name of the file system type.

static let volumeSubtypeKey: URLResourceKey

The key for the file system subtype value.

static let volumeMountFromLocationKey: URLResourceKey

The key for the volume mounted-from location.

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

static let volumeSupportsExtendedSecurityKey: URLResourceKey

Key for determining whether the volume supports extended security (access control lists), returned as a Boolean `NSNumber` object (read-only).

static let volumeSupportsFileCloningKey: URLResourceKey

Whether the volume supports cloning using `clonefile(2)`, returned as `NSNumber` containing a Boolean value (read-only).

static let volumeSupportsHardLinksKey: URLResourceKey

Key for determining whether the volume supports hard links, returned as a Boolean `NSNumber` object (read-only).

static let volumeSupportsImmutableFilesKey: URLResourceKey

static let volumeSupportsJournalingKey: URLResourceKey

Key for determining whether the volume supports journaling, returned as a Boolean `NSNumber` object (read-only).

static let volumeSupportsPersistentIDsKey: URLResourceKey

Key for determining whether the volume supports persistent IDs, returned as a Boolean `NSNumber` object (read-only).

static let volumeSupportsRenamingKey: URLResourceKey

Key for determining whether the volume can be renamed, returned as a Boolean `NSNumber` object (read-only).

static let volumeSupportsRootDirectoryDatesKey: URLResourceKey

Key for determining whether the volume supports reliable storage of times for the root directory, returned as a Boolean `NSNumber` object (read-only).

static let volumeSupportsSparseFilesKey: URLResourceKey

Key for determining whether the volume supports sparse files, returned as a Boolean `NSNumber` object (read-only).

static let volumeSupportsSwapRenamingKey: URLResourceKey

Whether the volume supports renaming using `renamex_np(2)` with the `RENAME_SWAP` option, returned as `NSNumber` containing a Boolean value (read-only).

static let volumeSupportsSymbolicLinksKey: URLResourceKey

Key for determining whether the volume supports symbolic links, returned as a Boolean `NSNumber` object (read-only).

static let volumeSupportsVolumeSizesKey: URLResourceKey

Key for determining whether the volume supports returning volume size information, returned as a Boolean `NSNumber` object (read-only). If `true`, volume size information is available as values of the volumeTotalCapacityKey andvolumeAvailableCapacityKey keys.

static let volumeSupportsZeroRunsKey: URLResourceKey

Key for determining whether the volume supports zero runs, returned as a Boolean `NSNumber` object (read-only).

static let volumeURLForRemountingKey: URLResourceKey

Key for the URL needed to remount the network volume, returned as an `NSURL` object, or `nil` if a URL is not available (read-only).

static let volumeURLKey: URLResourceKey

The root directory of the resource’s volume, returned as an `NSURL` object (read-only).

static let volumeUUIDStringKey: URLResourceKey

Key for the volume’s persistent UUID, returned as an `NSString` object, or `nil` if a persistent UUID is not available (read-only).

### Ubiquitous keys

Keys that describe the iCloud storage state of a file.

static let isUbiquitousItemKey: URLResourceKey

The key for a Boolean value that indicates whether the item is in iCloud storage.

static let ubiquitousSharedItemMostRecentEditorNameComponentsKey: URLResourceKey

The key for the name components of the most recent editor.

static let ubiquitousItemDownloadRequestedKey: URLResourceKey

The key for a Boolean value that indicates whether the system has already made a call startDownloadingUbiquitousItem(at:) to download the item.

static let ubiquitousItemIsDownloadingKey: URLResourceKey

The key for a Boolean value that indicates whether the system is downloading the item from iCloud.

static let ubiquitousItemDownloadingErrorKey: URLResourceKey

The key for an error object that indicates why downloading the item from iCloud fails.

static let ubiquitousItemDownloadingStatusKey: URLResourceKey

The key for the current download state for the item.

struct URLUbiquitousItemDownloadingStatus

Values that describe the iCloud storage state of a file.

static let ubiquitousItemIsExcludedFromSyncKey: URLResourceKey

The key of a Boolean value that indicates whether the system excludes the item from syncing.

static let ubiquitousItemIsUploadedKey: URLResourceKey

The key for a Boolean value that indicates whether the system uploads the item’s data to iCloud storage.

static let ubiquitousItemIsUploadingKey: URLResourceKey

The key for a Boolean value that indicates whether the system is uploading the item to iCloud.

static let ubiquitousItemUploadingErrorKey: URLResourceKey

The key for an error object that indicates why uploading the item to iCloud fails.

static let ubiquitousItemHasUnresolvedConflictsKey: URLResourceKey

The key for a Boolean value that indicates whether this item has outstanding conflicts.

static let ubiquitousItemContainerDisplayNameKey: URLResourceKey

The key for a string that contains the name of the item’s container as it appears to the user.

static let ubiquitousSharedItemOwnerNameComponentsKey: URLResourceKey

The key for the name components of the item’s owner.

static let ubiquitousSharedItemCurrentUserPermissionsKey: URLResourceKey

The key for the current user’s permissions.

static let ubiquitousSharedItemCurrentUserRoleKey: URLResourceKey

The key for the role of the current user.

static let ubiquitousItemIsSharedKey: URLResourceKey

The key for a Boolean value that indicates a shared item.

struct URLUbiquitousSharedItemRole

The key for the role of a shared item.

struct URLUbiquitousSharedItemPermissions

The key for the permissions of a shared item.

### Thumbnail keys

static let thumbnailKey: URLResourceKey

All thumbnails as a single NSImage (read-write).

Deprecated

static let thumbnailDictionaryKey: URLResourceKey

A dictionary of NSImage/UIImage objects keyed by size (read-write). See URLThumbnailDictionaryItem for a list of possible keys.

Deprecated

struct URLThumbnailDictionaryItem

Possible keys for the thumbnailDictionaryKey dictionary.

### Other resource keys

static let keysOfUnsetValuesKey: URLResourceKey

Key for the resource properties that have not been set after the setResourceValues(_:) method returns an error, returned as an array of `NSString` objects.

static let quarantinePropertiesKey: URLResourceKey

static let addedToDirectoryDateKey: URLResourceKey

The time at which the resource’s was created or renamed into or within its parent directory, returned as an `NSDate`. Inconsistent behavior may be observed when this attribute is requested on hard-linked items. This property is not supported by all volumes. (read-only)

static let attributeModificationDateKey: URLResourceKey

The time at which the resource’s attributes were most recently modified, returned as an `NSDate` object if the volume supports attribute modification dates, or `nil` if attribute modification dates are unsupported (read-only).

static let contentAccessDateKey: URLResourceKey

The time at which the resource was most recently accessed.

static let contentModificationDateKey: URLResourceKey

The time at which the resource was most recently modified.

static let creationDateKey: URLResourceKey

The time at which the resource was created.

static let customIconKey: URLResourceKey

The icon stored with the resource, returned as an `NSImage` object, or `nil` if the resource has no custom icon.

static let documentIdentifierKey: URLResourceKey

The document identifier returned as an `NSNumber` (read-only).

static let effectiveIconKey: URLResourceKey

The resource’s normal icon, returned as an `NSImage` object (read-only).

static let generationIdentifierKey: URLResourceKey

An opaque generation identifier, returned as an `id ` (read-only)

static let hasHiddenExtensionKey: URLResourceKey

Key for determining whether the resource’s extension is normally removed from its localized name, returned as a Boolean `NSNumber` object (read-write).

static let isExcludedFromBackupKey: URLResourceKey

A key for indicating whether the system excludes the resource from all backups of app data.

static let isExecutableKey: URLResourceKey

Key for determining whether the current process (as determined by the EUID) can execute the resource (if it is a file) or search the resource (if it is a directory), returned as a Boolean `NSNumber` object (read-only).

static let isHiddenKey: URLResourceKey

Key for determining whether the resource is normally not displayed to users, returned as a Boolean `NSNumber` object (read-write).

static let isReadableKey: URLResourceKey

Key for determining whether the current process (as determined by the EUID) can read the resource, returned as a Boolean `NSNumber` object (read-only).

static let isSymbolicLinkKey: URLResourceKey

Key for determining whether the resource is a symbolic link, returned as a Boolean `NSNumber` object (read-only).

static let isSystemImmutableKey: URLResourceKey

Key for determining whether the resource’s system immutable bit is set, returned as a Boolean `NSNumber` object (read-write).

static let isUserImmutableKey: URLResourceKey

Key for determining whether the resource’s user immutable bit is set, returned as a Boolean `NSNumber` object (read-write).

static let isWritableKey: URLResourceKey

Key for determining whether the current process (as determined by the EUID) can write to the resource, returned as a Boolean `NSNumber` object (read-only).

static let labelColorKey: URLResourceKey

The resource’s label color, returned as an `NSColor` object, or `nil` if the resource has no label color (read-only).

static let labelNumberKey: URLResourceKey

The resource’s label number, returned as an `NSNumber` object (read-write).

static let linkCountKey: URLResourceKey

The number of hard links to the resource, returned as an `NSNumber` object (read-only).

static let localizedLabelKey: URLResourceKey

The resource’s localized label text, returned as an `NSString` object, or `nil` if the resource has no localized label text (read-only).

static let localizedNameKey: URLResourceKey

The resource’s localized or extension-hidden name, returned as an `NSString` object (read-only).

static let localizedTypeDescriptionKey: URLResourceKey

The resource’s localized type description, returned as an `NSString` object (read-only).

static let nameKey: URLResourceKey

The resource’s name in the file system, returned as an `NSString` object (read-write).

static let pathKey: URLResourceKey

The file system path for the URL, returned as an NSString object (read-only).

static let canonicalPathKey: URLResourceKey

static let tagNamesKey: URLResourceKey

The names of tags attached to the resource, returned as an array of `NSString` values (read-write).

static let typeIdentifierKey: URLResourceKey

The resource’s uniform type identifier (UTI), returned as an `NSString` object (read-only).

Deprecated

static let contentTypeKey: URLResourceKey

The resource’s type.

### Initializers

init(String)

init(rawValue: String)

### Deprecated

static let ubiquitousItemIsDownloadedKey: URLResourceKey

The key for a Boolean value that indicates whether the system downloaded this item’s data from iCloud storage.

Deprecated

static let ubiquitousItemPercentDownloadedKey: URLResourceKey

The key for a value that indicates the percentage of data that the system downloaded from iCloud storage.

Deprecated

static let ubiquitousItemPercentUploadedKey: URLResourceKey

The key for a value that indicates the percentage of data that the system uploaded to iCloud storage.

Deprecated

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Resource Values

func resourceValues(forKeys: [URLResourceKey]) throws -> [URLResourceKey : Any]

Returns the resource values for the properties identified by specified array of keys.

func getResourceValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: URLResourceKey) throws

Returns the value of the resource property for the specified key.

func setResourceValue(Any?, forKey: URLResourceKey) throws

Sets the URL’s resource property for a given key to a given value.

func setResourceValues([URLResourceKey : Any]) throws

Sets the URL’s resource properties for a given set of keys to a given set of values.

func removeAllCachedResourceValues()

Removes all cached resource values and temporary resource values from the URL object.

func removeCachedResourceValue(forKey: URLResourceKey)

Removes the cached resource value identified by a given key from the URL object.

func setTemporaryResourceValue((any Sendable)?, forKey: URLResourceKey)

Sets a temporary resource value on the URL object.

