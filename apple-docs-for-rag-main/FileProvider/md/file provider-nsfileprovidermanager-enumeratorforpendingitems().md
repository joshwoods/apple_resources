

- File Provider
- NSFileProviderManager
-  enumeratorForPendingItems() 

Instance Method

# enumeratorForPendingItems()

Returns an enumerator for the set of pending items.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
func enumeratorForPendingItems() -> any NSFileProviderPendingSetEnumerator
```

## Discussion

When the set of pending items changes, the system calls pendingItemsDidChange(completionHandler:).

## See Also

### Working with items

func reimportItems(below: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Tells the system to reimport the item and its content recursively.

func evictItem(identifier: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Asks the system to remove an item from its cache.

func requestDownloadForItem(withIdentifier: NSFileProviderItemIdentifier, requestedRange: NSRange?) async throws

func requestDownloadForItem(withIdentifier: NSFileProviderItemIdentifier, requestedRange: NSRange?, completionHandler: ((any Error)?) -> Void)

func requestModification(of: NSFileProviderItemFields, forItemWithIdentifier: NSFileProviderItemIdentifier, options: NSFileProviderModifyItemOptions, completionHandler: ((any Error)?) -> Void)

func enumeratorForMaterializedItems() -> any NSFileProviderEnumerator

Returns an enumerator for all the items the system currently stores on disk.

