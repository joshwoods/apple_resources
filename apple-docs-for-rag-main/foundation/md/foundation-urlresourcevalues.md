

- Foundation
-  URLResourceValues 

Structure

# URLResourceValues

The properties that the file system resources support.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct URLResourceValues
```

## Overview

Not all property values exist for all file system URLs. For example, if a file is located on a volume that doesn’t support creation dates, you can request the creation date property, but the request returns `nil` and doesn’t generate an error.

Only the fields requested by the keys you pass into the `URL` function to receive this value will be populated. The other fields return `nil` regardless of the underlying property on the file system.

As a convenience, you can request volume resource values from any file system URL. The value returned reflects the property value for the volume that the resource is located on.

## Topics

### Application values

var applicationIsScriptable: Bool?

A Boolean value that indicates whether the application is scriptable.

var isApplication: Bool?

A Boolean value that indicates whether the resource is an application.

### Directory values

var isDirectory: Bool?

A Boolean value that indicates whether the resource is a directory.

var directoryEntryCount: Int?

The count of file system objects in the directory.

### File values

var documentIdentifier: Int?

A value that the kernel assigns to identify a document.

var fileContentIdentifier: Int64?

A value APFS assigns that identifies a file’s content data stream.

var fileAllocatedSize: Int?

The total allocated size on-disk for the file, in bytes.

var fileProtection: URLFileProtection?

The protection level for the file.

var fileResourceIdentifier: (any NSCopying &amp; NSSecureCoding &amp; NSObjectProtocol)?

An identifier for comparing two file system objects for equality.

var fileResourceType: URLFileResourceType?

The type of the file system object.

var fileSecurity: NSFileSecurity?

The file system object’s security information.

var fileSize: Int?

The total file size, in bytes.

var isPurgeable: Bool?

A Boolean value that indicates whether the file system can delete a file when the system needs to free space.

var isSparse: Bool?

A Boolean value that indicates whether the file has sparse regions.

var mayHaveExtendedAttributes: Bool?

A Boolean value that indicates the file may have extended attributes.

var isExecutable: Bool?

A Boolean value that indicates whether you can execute the file resource or search a directory resource.

var isRegularFile: Bool?

A Boolean value that indicates whether the resource is a regular file.

var mayShareFileContent: Bool?

A Boolean value that indicates whether the cloned files and their original files may share data blocks.

var totalFileAllocatedSize: Int?

The total allocated size of the file, in bytes.

var totalFileSize: Int?

The total displayable size of the file, in bytes.

var fileIdentifier: UInt64?

The file system’s internal inode identifier for the item.

### Volume capacity values

var volumeAvailableCapacity: Int?

The volume’s available capacity, in bytes.

var volumeAvailableCapacityForImportantUsage: Int64?

The volume’s available capacity for storing important resources, in bytes.

var volumeAvailableCapacityForOpportunisticUsage: Int64?

The volume’s available capacity for storing nonessential resources, in bytes.

var volumeTotalCapacity: Int?

The volume’s total capacity, in bytes.

### Volume status values

var volumeIsAutomounted: Bool?

A Boolean value that indicates whether the volume is automounted.

var volumeIsBrowsable: Bool?

A Boolean value that indicates whether the volume is visible through the user interface.

var volumeIsEjectable: Bool?

A Boolean value that indicates whether the volume’s media is ejectable from the drive mechanism under software control.

var volumeIsEncrypted: Bool?

A Boolean value that indicates whether the volume is encrypted.

var volumeIsInternal: Bool?

A Boolean value that indicates whether the volume’s device is connected to an internal bus, or nil if not available.

var volumeIsJournaling: Bool?

A Boolean value that indicates whether the volume is currently using a journal for speedy recovery after an unplanned restart.

var volumeIsLocal: Bool?

A Boolean value that indicates whether the volume is on a local device.

var volumeIsReadOnly: Bool?

A Boolean value that indicates whether the volume is read-only.

var volumeIsRemovable: Bool?

A Boolean value that indicates whether the volume’s media is removable from the drive mechanism.

var volumeIsRootFileSystem: Bool?

A Boolean value that indicates whether the volume is the root file system.

var volumeTypeName: String?

The volume’s type name, as a string.

var volumeSubtype: Int?

An integer value that indicates the file system subtype.

var volumeMountFromLocation: String?

The file system device location, as a string.

### Volume support values

var isMountTrigger: Bool?

A Boolean value that indicates whether this URL is a file system trigger directory.

var isVolume: Bool?

A Boolean value that indicates whether the root directory is a volume.

var volume: URL?

URL of the volume on which the resource is stored.

var volumeCreationDate: Date?

The volume’s creation date, or `nil` if this cannot be determined.

var volumeIdentifier: (any NSCopying &amp; NSSecureCoding &amp; NSObjectProtocol)?

An identifier that identifies the volume the file system object is on.

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

var volumeSupportsExtendedSecurity: Bool?

A Boolean value that indicates whether the volume implements extended security (ACLs).

var volumeSupportsFileCloning: Bool?

A Boolean value that indicates whether the volume supports file cloning.

var volumeSupportsHardLinks: Bool?

A Boolean value that indicates whether the volume format supports hard links.

var volumeSupportsImmutableFiles: Bool?

A Boolean value that indicates whether the volume supports making files immutable.

var volumeSupportsJournaling: Bool?

A Boolean value that indicates whether the volume format supports a journal used to speed recovery in case of unplanned restart (such as a power outage or crash).

var volumeSupportsPersistentIDs: Bool?

A Boolean value that indicates whether the volume format supports persistent object identifiers and can look up file system objects by their IDs.

var volumeSupportsRenaming: Bool?

A Boolean value that indicates whether the volume can be renamed.

var volumeSupportsRootDirectoryDates: Bool?

A Boolean value that indicates whether the volume supports reliable storage of times for the root directory.

var volumeSupportsSparseFiles: Bool?

A Boolean value that indicates whether the volume format supports sparse files.

var volumeSupportsSwapRenaming: Bool?

A Boolean value that indicates whether the volume supports swapping source and target files when both exist.

var volumeSupportsSymbolicLinks: Bool?

A Boolean value that indicates whether the volume format supports symbolic links.

var volumeSupportsVolumeSizes: Bool?

A Boolean value that indicates whether the volume supports returning volume size values.

var volumeSupportsZeroRuns: Bool?

A Boolean value that indicates whether the volume keeps track of allocated but unwritten parts of a file so that it can substitute zeroes without actually writing zeroes to the media.

var volumeURLForRemounting: URL?

The `URL` needed to remount a network volume, or `nil` if not available.

var volumeUUIDString: String?

The volume’s persistent `UUID` as a string, or `nil` if a persistent `UUID` is not available for the volume.

### Ubiquitous values

var isUbiquitousItem: Bool?

A Boolean value that indicates whether the item is in the iCloud storage.

var ubiquitousItemIsShared: Bool?

A Boolean value that indicates a shared item.

var ubiquitousItemIsExcludedFromSync: Bool?

A Boolean value that indicates the system excludes the item from syncing.

var ubiquitousSharedItemCurrentUserPermissions: URLUbiquitousSharedItemPermissions?

The current user’s permissions for the shared item.

var ubiquitousSharedItemCurrentUserRole: URLUbiquitousSharedItemRole?

The current user’s role for the shared item.

var ubiquitousSharedItemMostRecentEditorNameComponents: PersonNameComponents?

The name components of the most recent editor of the shared item.

var ubiquitousSharedItemOwnerNameComponents: PersonNameComponents?

The name components of the owner of the shared item.

var ubiquitousItemContainerDisplayName: String?

The name of the item’s container as the system displays it to users.

var ubiquitousItemDownloadRequested: Bool?

A Boolean value that indicates whether the user or the system requests a download of the item.

var ubiquitousItemDownloadingError: NSError?

The error when downloading the item from iCloud fails.

var ubiquitousItemDownloadingStatus: URLUbiquitousItemDownloadingStatus?

The download status of the item.

var ubiquitousItemHasUnresolvedConflicts: Bool?

A Boolean value that indicates whether the item has outstanding conflicts.

var ubiquitousItemIsDownloading: Bool?

A Boolean value that indicates whether the system is downloading the item.

var ubiquitousItemIsUploaded: Bool?

A Boolean value that indicates whether data is present in the cloud for the item.

var ubiquitousItemIsUploading: Bool?

A Boolean value that indicates whether the system is uploading the item.

var ubiquitousItemUploadingError: NSError?

The error when uploading the item to iCloud fails.

### Thumbnail values

var thumbnail: NSImage?

A thumbnail image of the URL.

Deprecated

var thumbnailDictionary: [URLThumbnailDictionaryItem : UIImage]?

A dictionary of UIKit image objects keyed by size.

Deprecated

var thumbnailDictionary: [URLThumbnailDictionaryItem : NSImage]?

A dictionary of AppKit image objects keyed by size.

Deprecated

### Universal resource values

var addedToDirectoryDate: Date?

The date the resource was created, or renamed into or within its parent directory.

var allValues: [URLResourceKey : Any]

A loosely-typed dictionary containing all keys and values.

var attributeModificationDate: Date?

The time the resource’s attributes were last modified.

var canonicalPath: String?

The URL’s path as a canonical absolute file system path.

var contentAccessDate: Date?

The date the resource was last accessed.

var contentModificationDate: Date?

The time the resource content was last modified.

var creationDate: Date?

The date the resource was created.

var customIcon: NSImage?

var effectiveIcon: AnyObject?

var generationIdentifier: (any NSCopying &amp; NSSecureCoding &amp; NSObjectProtocol)?

An opaque generation identifier which can be compared using `==` to determine if the data in a document has been modified.

var hasHiddenExtension: Bool?

True for resources whose filename extension is removed from the localized name property.

var isAliasFile: Bool?

true if the resource is a Finder alias file or a symlink, false otherwise

var isExcludedFromBackup: Bool?

True if resource should be excluded from backups, false otherwise.

var isHidden: Bool?

True for resources normally not displayed to users.

var isPackage: Bool?

True for packaged directories.

var isReadable: Bool?

True if this process (as determined by EUID) can read the resource.

var isSymbolicLink: Bool?

True for symlinks.

var isSystemImmutable: Bool?

True for system-immutable resources.

var isUserImmutable: Bool?

True for user-immutable resources

var isWritable: Bool?

True if this process (as determined by EUID) can write to the resource.

var labelColor: NSColor?

var labelNumber: Int?

The label number assigned to the resource.

var linkCount: Int?

Number of hard links to the resource.

var localizedLabel: String?

The user-visible label text.

var localizedName: String?

Localized or extension-hidden name as displayed to users.

var localizedTypeDescription: String?

User-visible type or “kind” description.

var name: String?

The resource name provided by the file system.

var parentDirectory: URL?

The resource’s parent directory, if any.

var path: String?

The URL’s path as a file system path.

var preferredIOBlockSize: Int?

The optimal block size when reading or writing this file’s data, or nil if not available.

var quarantineProperties: [String : Any]?

The quarantine properties as defined in LSQuarantine.h. To remove quarantine information from a file, pass `nil` as the value when setting this property.

var tagNames: [String]?

The array of Tag names.

var typeIdentifier: String?

A string that represents the identifier for the type of the resource.

Deprecated

var contentType: UTType?

The resource’s type.

### Initializers

init()

Initializes a new resource values structure.

## See Also

### Accessing resource values

func resourceValues(forKeys: Set&lt;URLResourceKey>) throws -> URLResourceValues

Returns a collection of resource values identified by the given resource keys.

func setResourceValues(URLResourceValues) throws

Sets the resource value identified by a given resource key.

func removeCachedResourceValue(forKey: URLResourceKey)

Removes the cached resource value identified by a given resource value key from the URL object.

func removeAllCachedResourceValues()

Removes all cached resource values and all temporary resource values from the URL object.

func setTemporaryResourceValue(any Sendable, forKey: URLResourceKey)

Sets a temporary resource value on the URL object.

struct URLResourceKey

Keys that apply to file system URLs.

