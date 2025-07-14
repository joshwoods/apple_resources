

- File Provider
- NSFileProviderExtension
-  item(for:) 

Instance Method

# item(for:)

Returns a description of the item associated with the persistent identifier.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
func item(for identifier: NSFileProviderItemIdentifier) throws -> NSFileProviderItem
```

## Parameters 

`identifier`  

The persistent identifier for a shared document.

## Return Value

A custom object that describes the specified document or directory, or `nil` in Objective-C if an error occurs.

## Discussion

Your File Provider extension must define a class that adopts the NSFileProviderItemProtocol interface. Instances of this class provides access to information about an item (a document or directory) that your File Provider manages and stores.

Your class should implement as many of the protocol’s optional methods as makes sense for the specified item. This lets the system provide as much information as possible to the user as they browse your File Provider.

Optionally, you can define different classes for different types of items—for example, different classes for documents and directories. These classes can define different subsets of the NSFileProviderItemProtocol interface’s optional methods. For example, the class representing a folder implements the childItemCount property, while the class representing a document does not.

Override this method to look up the item associated with the persistent identifier and return an instance of your custom NSFileProviderItemProtocol class for that item.

## See Also

### Working with items and persistent identifiers

func persistentIdentifierForItem(at: URL) -> NSFileProviderItemIdentifier?

Returns a unique identifier for the given URL.

func urlForItem(withPersistentIdentifier: NSFileProviderItemIdentifier) -> URL?

Returns the URL for a given persistent identifier.

func enumerator(for: NSFileProviderItemIdentifier) throws -> any NSFileProviderEnumerator

Returns an enumerator for the specified item.

struct NSFileProviderItemIdentifier

A unique identifier for an item managed by the File Provider extension.

