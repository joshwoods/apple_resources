

- File Provider
- NSFileProviderItemCapabilities
-  allowsAll Deprecated

Type Property

# allowsAll

A convenience value for enabling all capabilities.

iOS 11.0–15.0DeprecatediPadOS 11.0–15.0DeprecatedmacOS 11.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static var allowsAll: NSFileProviderItemCapabilities { get }
```

Deprecated

This capability is no longer supported, and does not contain all capabilities. Please migrate to directly specifying each of the individual capabilities that should be allowed for the item.

## See Also

### Constants

static var allowsAddingSubItems: NSFileProviderItemCapabilities

A value indicating that the user can add subitems.

static var allowsContentEnumerating: NSFileProviderItemCapabilities

A value indicating that the item’s contents can be enumerated.

static var allowsDeleting: NSFileProviderItemCapabilities

A value indicating that the item can be deleted.

static var allowsEvicting: NSFileProviderItemCapabilities

A value indicating that the system can delete the local copy of the item.

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

