

- File Provider
- NSFileProviderManager
-  requestDownloadForItem(withIdentifier:requestedRange:completionHandler:) 

Instance Method

# requestDownloadForItem(withIdentifier:requestedRange:completionHandler:)

iOS 16.0+iPadOS 16.0+macOS 13.0+visionOS 1.0+

``` source
func requestDownloadForItem(
    withIdentifier itemIdentifier: NSFileProviderItemIdentifier,
    requestedRange: NSRange? = nil,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

## See Also

### Working with items

func reimportItems(below: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Tells the system to reimport the item and its content recursively.

func evictItem(identifier: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Asks the system to remove an item from its cache.

func requestDownloadForItem(withIdentifier: NSFileProviderItemIdentifier, requestedRange: NSRange?) async throws

func requestModification(of: NSFileProviderItemFields, forItemWithIdentifier: NSFileProviderItemIdentifier, options: NSFileProviderModifyItemOptions, completionHandler: ((any Error)?) -> Void)

func enumeratorForMaterializedItems() -> any NSFileProviderEnumerator

Returns an enumerator for all the items the system currently stores on disk.

func enumeratorForPendingItems() -> any NSFileProviderPendingSetEnumerator

Returns an enumerator for the set of pending items.

