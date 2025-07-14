

- File Provider
- NSFileProviderManager
-  requestDownloadForItemWithIdentifier:requestedRange:completionHandler: 

Instance Method

# requestDownloadForItemWithIdentifier:requestedRange:completionHandler:

macOS 13.0+

``` source
- (void) requestDownloadForItemWithIdentifier:(NSFileProviderItemIdentifier) itemIdentifier 
                               requestedRange:(NSRange) rangeToMaterialize 
                            completionHandler:(void (^)(NSError * error)) completionHandler;
```

## See Also

### Working with items

func reimportItems(below: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Tells the system to reimport the item and its content recursively.

func evictItem(identifier: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Asks the system to remove an item from its cache.

func requestModification(of: NSFileProviderItemFields, forItemWithIdentifier: NSFileProviderItemIdentifier, options: NSFileProviderModifyItemOptions, completionHandler: ((any Error)?) -> Void)

func enumeratorForMaterializedItems() -> any NSFileProviderEnumerator

Returns an enumerator for all the items the system currently stores on disk.

func enumeratorForPendingItems() -> any NSFileProviderPendingSetEnumerator

Returns an enumerator for the set of pending items.

