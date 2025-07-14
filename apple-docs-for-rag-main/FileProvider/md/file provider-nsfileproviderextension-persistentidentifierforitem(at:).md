

- File Provider
- NSFileProviderExtension
-  persistentIdentifierForItem(at:) 

Instance Method

# persistentIdentifierForItem(at:)

Returns a unique identifier for the given URL.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
func persistentIdentifierForItem(at url: URL) -> NSFileProviderItemIdentifier?
```

## Parameters 

`url`  

The URL of a shared document.

## Return Value

A unique identifier for the item specified by the URL, or `nil` if the document is not in the File Provider’s shared container.

## Discussion

Override this method to define a static mapping between URLs and their persistent identifiers. A document’s identifier should remain constant over time; it should not change when the document is edited, moved, or renamed.

For example, if you already have a unique key for the document in your cloud database, you can use that key as the document’s identifier.

Always return `nil` if the URL is not inside in the directory referred to by the NSFileProviderManager object’s documentStorageURL property.

## See Also

### Working with items and persistent identifiers

func urlForItem(withPersistentIdentifier: NSFileProviderItemIdentifier) -> URL?

Returns the URL for a given persistent identifier.

func item(for: NSFileProviderItemIdentifier) throws -> NSFileProviderItem

Returns a description of the item associated with the persistent identifier.

func enumerator(for: NSFileProviderItemIdentifier) throws -> any NSFileProviderEnumerator

Returns an enumerator for the specified item.

struct NSFileProviderItemIdentifier

A unique identifier for an item managed by the File Provider extension.

