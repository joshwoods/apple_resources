

- File Provider
- NSFileProviderItemCapabilities
-  allowsEvicting 

Type Property

# allowsEvicting

A value indicating that the system can delete the local copy of the item.

iOS 11.0+iPadOS 11.0+macOS 11.0–13.0DeprecatedvisionOS 1.0+

``` source
static var allowsEvicting: NSFileProviderItemCapabilities { get }
```

## See Also

### Constants

static var allowsAddingSubItems: NSFileProviderItemCapabilities

A value indicating that the user can add subitems.

static var allowsContentEnumerating: NSFileProviderItemCapabilities

A value indicating that the item’s contents can be enumerated.

static var allowsDeleting: NSFileProviderItemCapabilities

A value indicating that the item can be deleted.

static var allowsReading: NSFileProviderItemCapabilities

A value indicating that the value can be read from.

static var allowsRenaming: NSFileProviderItemCapabilities

A value indicating that the item can be renamed.

static var allowsReparenting: NSFileProviderItemCapabilities

A value indicating that the item can be moved.

static var allowsTrashing: NSFileProviderItemCapabilities

A value indicating that the item can be moved to the trash.

static var allowsWriting: NSFileProviderItemCapabilities

A value indicating that the item can be written to.

static var allowsExcludingFromSync: NSFileProviderItemCapabilities

A value indicating that the user can exclude the item from sync operations.

static var allowsAll: NSFileProviderItemCapabilities

A convenience value for enabling all capabilities.

Deprecated

