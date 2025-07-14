

- File Provider
- NSFileProviderError
-  filenameCollision 

Type Property

# filenameCollision

An error indicating that an item with the same name already exists in the same directory.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
static var filenameCollision: NSFileProviderError.Code { get }
```

## Discussion

Use the fileProviderErrorForCollision(with:) method to create properly formatted filenameCollision errors.

You have two options for resolving file name collisions:

- Your file provider extension can return this error. In this case the system renames the new item.

- You can rename the new item yourself. This gives you complete control over the process.

## See Also

### Accessing error codes

enum Code

The error codes for the File Provider extension.

static var insufficientQuota: NSFileProviderError.Code

An error indicating that the File Provider extension can’t upload the item because it would push the account over its quota.

static var noSuchItem: NSFileProviderError.Code

An error indicating that the specified item doesn’t exist.

static var notAuthenticated: NSFileProviderError.Code

An error indicating that you can’t verify the user’s credentials.

static var pageExpired: NSFileProviderError.Code

An error indicating that the page is too old, and that the system must restart the enumeration operation from the beginning.

static var serverUnreachable: NSFileProviderError.Code

An error indicating that the File Provider extension can’t reach the remote server.

static var syncAnchorExpired: NSFileProviderError.Code

An error indicating that the sync anchor is too old, and that the system must restart the sync operation from the beginning.

static var directoryNotEmpty: NSFileProviderError.Code

An error indicating an attempt to nonrecursively delete a directory that isn’t empty.

static var providerNotFound: NSFileProviderError.Code

An error indicating that the File Provider manager can’t find the specified provider.

static var providerTranslocated: NSFileProviderError.Code

An error indicating the File Provider extension is in a disabled state due to Gatekeeper’s restrictions for apps from outside the App Store.

static var olderExtensionVersionRunning: NSFileProviderError.Code

An error indicating that the registered provider in the system is an older version than the one the app uses.

static var newerExtensionVersionFound: NSFileProviderError.Code

An error indicating that the registered provider in the system is a newer version than the one the app uses.

static var nonEvictable: NSFileProviderError.Code

An error indicating that the File Provider extension can’t evict an item.

static var nonEvictableChildren: NSFileProviderError.Code

An error indicating that the File Provider extension can’t evict a directory because it contains nonevictable items.

static var unsyncedEdits: NSFileProviderError.Code

An error indicating that the item contains unsynced changes.

