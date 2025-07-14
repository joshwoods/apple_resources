

- File Provider
- NSFileProviderManager
-  requestModification(of:forItemWithIdentifier:options:completionHandler:) 

Instance Method

# requestModification(of:forItemWithIdentifier:options:completionHandler:)

iOS 16.0+iPadOS 16.0+macOS 13.0+visionOS 1.0+

``` source
func requestModification(
    of fields: NSFileProviderItemFields,
    forItemWithIdentifier itemIdentifier: NSFileProviderItemIdentifier,
    options: NSFileProviderModifyItemOptions = [],
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func requestModification(
    of fields: NSFileProviderItemFields,
    forItemWithIdentifier itemIdentifier: NSFileProviderItemIdentifier,
    options: NSFileProviderModifyItemOptions = []
) async throws
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func requestModification(of fields: NSFileProviderItemFields, forItemWithIdentifier itemIdentifier: NSFileProviderItemIdentifier, options: NSFileProviderModifyItemOptions = []) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Working with items

func reimportItems(below: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Tells the system to reimport the item and its content recursively.

func evictItem(identifier: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Asks the system to remove an item from its cache.

func requestDownloadForItem(withIdentifier: NSFileProviderItemIdentifier, requestedRange: NSRange?) async throws

func requestDownloadForItem(withIdentifier: NSFileProviderItemIdentifier, requestedRange: NSRange?, completionHandler: ((any Error)?) -> Void)

func enumeratorForMaterializedItems() -> any NSFileProviderEnumerator

Returns an enumerator for all the items the system currently stores on disk.

func enumeratorForPendingItems() -> any NSFileProviderPendingSetEnumerator

Returns an enumerator for the set of pending items.

