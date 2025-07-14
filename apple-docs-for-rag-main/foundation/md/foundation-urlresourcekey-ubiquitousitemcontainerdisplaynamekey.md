

- Foundation
- URLResourceKey
-  ubiquitousItemContainerDisplayNameKey 

Type Property

# ubiquitousItemContainerDisplayNameKey

The key for a string that contains the name of the item’s container as it appears to the user.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let ubiquitousItemContainerDisplayNameKey: URLResourceKey
```

## See Also

### Ubiquitous keys

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

static let ubiquitousSharedItemOwnerNameComponentsKey: URLResourceKey

The key for the name components of the item’s owner.

static let ubiquitousSharedItemCurrentUserPermissionsKey: URLResourceKey

The key for the current user’s permissions.

static let ubiquitousSharedItemCurrentUserRoleKey: URLResourceKey

The key for the role of the current user.

