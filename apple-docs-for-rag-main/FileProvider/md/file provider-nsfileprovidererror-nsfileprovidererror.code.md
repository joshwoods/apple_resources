

- File Provider
- NSFileProviderError
-  NSFileProviderError.Code 

Enumeration

# NSFileProviderError.Code

The error codes for the File Provider extension.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error codes

case filenameCollision

An error indicating that an item with the same name already exists in the same directory.

case insufficientQuota

An error indicating that the File Provider extension can’t upload the item because it would push the account over its quota.

case noSuchItem

An error indicating that the specified item doesn’t exist.

case notAuthenticated

An error indicating that you can’t verify the user’s credentials.

case serverUnreachable

An error indicating that the File Provider extension can’t reach the remote server.

case syncAnchorExpired

An error indicating that the sync anchor is too old, and that the system must restart the sync operation from the beginning.

static var pageExpired: NSFileProviderError.Code

An error indicating that the page is too old, and that the system must restart the enumeration operation from the beginning.

case directoryNotEmpty

An error indicating an attempt to nonrecursively delete a directory that isn’t empty.

case providerNotFound

An error indicating that the File Provider manager can’t find the specified provider.

case providerTranslocated

An error indicating the File Provider extension is in a disabled state due to Gatekeeper’s restrictions for apps from outside the App Store.

case olderExtensionVersionRunning

An error indicating that the registered provider in the system is an older version than the one the app uses.

case newerExtensionVersionFound

An error indicating that the registered provider in the system is a newer version than the one the app uses.

case nonEvictable

An error indicating that the File Provider extension can’t evict an item.

case nonEvictableChildren

An error indicating that the File Provider extension can’t evict a directory because it contains nonevictable items.

case unsyncedEdits

An error indicating that the item contains unsynced changes.

case cannotSynchronize

An error indicating a failed sync attempt.

case deletionRejected

An error indicating a failed deletion action.

case versionNoLongerAvailable

An error indicating that the specified version is no longer available.

case domainDisabled

case excludedFromSync

case applicationExtensionNotFound

An error indicating that there isn’t an app extension within the app bundle.

case providerDomainNotFound

An error indicating that there isn’t a registered domain for the corresponding identifier.

case providerDomainTemporarilyUnavailable

An error indicating that the system is unable to service requests for the domain temporarily, and you can try again later.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct NSFileProviderError

A structure that contains information about File Provider extension errors.

let NSFileProviderErrorDomain: String

The error domain for the File Provider extension.

let NSFileProviderErrorItemKey: String

The key for accessing information about sync-related errors.

let NSFileProviderErrorNonExistentItemIdentifierKey: String

The key for accessing the specified item’s identifier when the item doesn’t exist.

let NSFileProviderErrorCollidingItemKey: String

The key for accessing the existing item from a filename collision error’s user info dictionary.

Deprecated

