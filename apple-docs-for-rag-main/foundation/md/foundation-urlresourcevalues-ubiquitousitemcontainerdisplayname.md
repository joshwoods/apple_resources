

- Foundation
- URLResourceValues
-  ubiquitousItemContainerDisplayName 

Instance Property

# ubiquitousItemContainerDisplayName

The name of the item’s container as the system displays it to users.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var ubiquitousItemContainerDisplayName: String? { get }
```

## See Also

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

