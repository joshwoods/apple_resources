

- File Provider
-  NSFileProviderExtension 

Class

# NSFileProviderExtension

The principal class for the nonreplicated File Provider extension.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
class NSFileProviderExtension
```

## Overview

To create a nonreplicated File Provider extension, start by creating a subclass of the NSFileProviderExtension class. When implementing your NSFileProviderExtension subclass, remember:

- Override all of the extension’s methods (except the deprecated methods), even if your implementation is only an empty method.

- Use your method implementations to provide access to the documents and folders managed by your file provider.

- Don’t call `super` in your method implementations.

Don’t use the NSFileProviderExtension class in macOS. Instead, create an NSObject subclass that adopts the NSFileProviderReplicatedExtension and NSFileProviderEnumerating protocols. For more information, see Replicated File Provider extension.

## Topics

### Working with items and persistent identifiers

func persistentIdentifierForItem(at: URL) -> NSFileProviderItemIdentifier?

Returns a unique identifier for the given URL.

func urlForItem(withPersistentIdentifier: NSFileProviderItemIdentifier) -> URL?

Returns the URL for a given persistent identifier.

func item(for: NSFileProviderItemIdentifier) throws -> NSFileProviderItem

Returns a description of the item associated with the persistent identifier.

func enumerator(for: NSFileProviderItemIdentifier) throws -> any NSFileProviderEnumerator

Returns an enumerator for the specified item.

struct NSFileProviderItemIdentifier

A unique identifier for an item managed by the File Provider extension.

### Managing shared files

func itemChanged(at: URL)

Tells the File Provider extension that a document has changed.

func providePlaceholder(at: URL, completionHandler: ((any Error)?) -> Void)

Triggers the creation of a placeholder for the given URL.

func startProvidingItem(at: URL, completionHandler: ((any Error)?) -> Void)

Provides an actual file on disk for a placeholder.

func stopProvidingItem(at: URL)

Tells the File Provider extension that a given document is no longer being accessed.

### Handling actions

Providing support for user-driven actions

Override methods to handle user-initiated actions.

func createDirectory(withName: String, inParentItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Creates a directory with the given name inside the given parent directory.

func deleteItem(withIdentifier: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Permanently deletes an item from the trash.

func importDocument(at: URL, toParentItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Imports a file or package into the given parent directory.

func renameItem(withIdentifier: NSFileProviderItemIdentifier, toName: String, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Renames a document or directory.

func reparentItem(withIdentifier: NSFileProviderItemIdentifier, toParentItemWithIdentifier: NSFileProviderItemIdentifier, newName: String?, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Moves the specified item into the given parent directory.

func setFavoriteRank(NSNumber?, forItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Marks a directory as a favorite and sets its relative order in the Favorites list.

func setLastUsedDate(Date?, forItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Marks an item as recently used and sets its relative order in the Recents list.

func setTagData(Data?, forItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Tags an item.

func trashItem(withIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Moves an item into the trash.

func untrashItem(withIdentifier: NSFileProviderItemIdentifier, toParentItemIdentifier: NSFileProviderItemIdentifier?, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Moves an item out of the trash.

### Managing domains

var domain: NSFileProviderDomain?

The domain managed by this file provider object.

### Accessing thumbnails

func fetchThumbnails(for: [NSFileProviderItemIdentifier], requestedSize: CGSize, perThumbnailCompletionHandler: (NSFileProviderItemIdentifier, Data?, (any Error)?) -> Void, completionHandler: ((any Error)?) -> Void) -> Progress

Fetches the thumbnails for items that have been enumerated by the file provider.

### Working with services

func supportedServiceSources(for: NSFileProviderItemIdentifier) throws -> [any NSFileProviderServiceSource]

Return an array of service sources that let the host app perform actions associated with the specified item.

protocol NSFileProviderServiceSource

A service that provides a custom communication channel between the host app and the File Provider extension.

### Managing placeholders

These methods have been deprecated and moved to the NSFileProviderManager class.

class func placeholderURL(for: URL) -> URL

Returns a placeholder URL for a given document URL.

Deprecated

class func writePlaceholder(at: URL, withMetadata: [URLResourceKey : Any]) throws

Writes a document placeholder with the provided metadata.

Deprecated

### Accessing the document storage

These methods have been deprecated and moved to the NSFileProviderManager class.

var documentStorageURL: URL

The root URL for all shared documents.

Deprecated

var providerIdentifier: String

A purpose identifier for coordinated reads and writes.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Nonreplicated extension

Content and Change Tracking

Create enumerators to specify your file provider’s content, and track changes to that content.

