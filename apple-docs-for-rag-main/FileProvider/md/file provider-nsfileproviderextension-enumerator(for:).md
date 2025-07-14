

- File Provider
- NSFileProviderExtension
-  enumerator(for:) 

Instance Method

# enumerator(for:)

Returns an enumerator for the specified item.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
func enumerator(for containerItemIdentifier: NSFileProviderItemIdentifier) throws -> any NSFileProviderEnumerator
```

## Parameters 

`containerItemIdentifier`  

The persistent identifier for a document or folder.

## Return Value

An enumerator for the specified document or folder, or `nil` in Objective-C if an error has occurred.

## Mentioned in 

Defining Your File Provider’s Content

## Discussion

Your File Provider extension must define one or more classes that adopt the NSFileProviderEnumerator protocol. Instances of these classes must be able to enumerate both the contents of the specified item and any changes to the content.

Override this method to return an instance of your custom NSFileProviderEnumerator class for the specified item (either a document or a folder). For more information, see Content and Change Tracking.

## See Also

### Working with items and persistent identifiers

func persistentIdentifierForItem(at: URL) -> NSFileProviderItemIdentifier?

Returns a unique identifier for the given URL.

func urlForItem(withPersistentIdentifier: NSFileProviderItemIdentifier) -> URL?

Returns the URL for a given persistent identifier.

func item(for: NSFileProviderItemIdentifier) throws -> NSFileProviderItem

Returns a description of the item associated with the persistent identifier.

struct NSFileProviderItemIdentifier

A unique identifier for an item managed by the File Provider extension.

