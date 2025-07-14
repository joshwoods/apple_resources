

- File Provider
- NSFileProviderItemCapabilities
-  allowsExcludingFromSync 

Type Property

# allowsExcludingFromSync

A value indicating that the user can exclude the item from sync operations.

macOS 11.3+

``` source
static var allowsExcludingFromSync: NSFileProviderItemCapabilities { get }
```

## Discussion

The user can choose to exclude the item from syncs (for example, in Finder’s user interface). If the user excludes an item, the system stops monitoring changes for the item and its children, and removes the item from the file provider.

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

static var allowsAll: NSFileProviderItemCapabilities

A convenience value for enabling all capabilities.

Deprecated

