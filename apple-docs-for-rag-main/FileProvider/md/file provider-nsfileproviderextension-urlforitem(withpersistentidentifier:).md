

- File Provider
- NSFileProviderExtension
-  urlForItem(withPersistentIdentifier:) 

Instance Method

# urlForItem(withPersistentIdentifier:)

Returns the URL for a given persistent identifier.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
func urlForItem(withPersistentIdentifier identifier: NSFileProviderItemIdentifier) -> URL?
```

## Parameters 

`identifier`  

The persistent identifier for a shared document.

## Return Value

The URL of a shared document.

## Discussion

Override this method to provide the URL for the document with the given identifier. This method must be the inverse of persistentIdentifierForItem(at:), mapping from the persistent identifier, back to the URL.

This URL must be inside the directory referred to by the NSFileProviderManager object’s documentStorageURL property.

## See Also

### Working with items and persistent identifiers

func persistentIdentifierForItem(at: URL) -> NSFileProviderItemIdentifier?

Returns a unique identifier for the given URL.

func item(for: NSFileProviderItemIdentifier) throws -> NSFileProviderItem

Returns a description of the item associated with the persistent identifier.

func enumerator(for: NSFileProviderItemIdentifier) throws -> any NSFileProviderEnumerator

Returns an enumerator for the specified item.

struct NSFileProviderItemIdentifier

A unique identifier for an item managed by the File Provider extension.

