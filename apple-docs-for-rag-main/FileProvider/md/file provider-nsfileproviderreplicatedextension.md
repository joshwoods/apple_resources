

- File Provider
-  NSFileProviderReplicatedExtension 

Protocol

# NSFileProviderReplicatedExtension

A File Provider extension in which the system replicates the contents on disk.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderReplicatedExtension : NSFileProviderEnumerating
```

## Mentioned in 

Using push notifications to signal changes

## Topics

### Creating and Removing File Providers

init(domain: NSFileProviderDomain)

Creates an instance of the file provider for the specified domain.

**Required**

func invalidate()

Tells the file provider to perform any necessary cleanup so that the system can deallocate it.

**Required**

### Accessing Remote Content

func item(for: NSFileProviderItemIdentifier, request: NSFileProviderRequest, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void) -> Progress

Asks the file provider for the metadata of the provided item.

**Required**

func fetchContents(for: NSFileProviderItemIdentifier, version: NSFileProviderItemVersion?, request: NSFileProviderRequest, completionHandler: (URL?, NSFileProviderItem?, (any Error)?) -> Void) -> Progress

Tells the file provider to download the requested item from remote storage.

**Required**

### Managing Items

func createItem(basedOn: NSFileProviderItem, fields: NSFileProviderItemFields, contents: URL?, options: NSFileProviderCreateItemOptions, request: NSFileProviderRequest, completionHandler: (NSFileProviderItem?, NSFileProviderItemFields, Bool, (any Error)?) -> Void) -> Progress

Tells the file provider to create or import an item based on a template.

**Required**

struct NSFileProviderCreateItemOptions

Options for creating items.

func modifyItem(NSFileProviderItem, baseVersion: NSFileProviderItemVersion, changedFields: NSFileProviderItemFields, contents: URL?, options: NSFileProviderModifyItemOptions, request: NSFileProviderRequest, completionHandler: (NSFileProviderItem?, NSFileProviderItemFields, Bool, (any Error)?) -> Void) -> Progress

Tells the file provider that an item’s content or metadata changed.

**Required**

struct NSFileProviderModifyItemOptions

Options for modifying items.

func deleteItem(identifier: NSFileProviderItemIdentifier, baseVersion: NSFileProviderItemVersion, options: NSFileProviderDeleteItemOptions, request: NSFileProviderRequest, completionHandler: ((any Error)?) -> Void) -> Progress

Tells the file provider to delete an item forever.

**Required**

struct NSFileProviderDeleteItemOptions

Options for deleting items.

### Tracking Materialized Items

func materializedItemsDidChange(completionHandler: () -> Void)

Tells the file provider that the set of materialized items changed.

### Tracking Pending Items

func pendingItemsDidChange(completionHandler: () -> Void)

Tells the file provider extension that the set of pending items has changed.

### Importing Domains

func importDidFinish(completionHandler: () -> Void)

Tells the File Provider extension that the system finished importing items.

## Relationships

### Inherits From

- NSFileProviderEnumerating
- NSObjectProtocol

## See Also

### File Provider protocols

protocol NSFileProviderEnumerating

Support for enumerating the file provider’s contents.

protocol NSFileProviderIncrementalContentFetching

Support for fetching changes to the item’s content.

protocol NSFileProviderPartialContentFetching

Support for fetching part of a file’s content.

protocol NSFileProviderServicing

Support for providing a custom service source.

protocol NSFileProviderCustomAction

Support for custom actions.

struct NSFileProviderExtensionActionIdentifier

An identifier for custom actions.

protocol NSFileProviderThumbnailing

Support for item thumbnails.

protocol NSFileProviderPendingSetEnumerator

A protocol for enumerating pending items.

