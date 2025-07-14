

- File Provider
- NSFileProviderManager
-  evictItem(identifier:completionHandler:) 

Instance Method

# evictItem(identifier:completionHandler:)

Asks the system to remove an item from its cache.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func evictItem(
    identifier itemIdentifier: NSFileProviderItemIdentifier,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func evictItem(identifier itemIdentifier: NSFileProviderItemIdentifier) async throws
```

## Parameters 

`itemIdentifier`  

The item’s identifier.

`completionHandler`  

A block that the system calls after removing the item from disk. The system passes the following parameter:

`error`  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func evictItem(identifier itemIdentifier: NSFileProviderItemIdentifier) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Calling this method turns a materialized item into a dataless item to free up disk space. For more information on materialized and dataless items, see Synchronizing the File Provider Extension.

If the item is a document without local changes, this method deletes the local copy of the item’s content. If the item has local changes, it fails with an NSFileWriteNoPermissionError error.

When called on a directory, the system recursively evicts the directory’s content. It deletes the content of any materialized files, and recursively evicts any subdirectories. After it has successfully evicted all the content, it deletes its list of the directory’s content, making the directory dataless. The next time the system accesses the directory, it requests a list of the contents using the NSFileProviderEnumerating protocol.

If the system encounters a nonevictable child, eviction stops immediately, and the system calls the completion handler with a NSFileProviderError.Code.nonEvictableChildren error. The error includes information about the nonevictable child in its underlyingErrors property. The system may have evicted other materialized items, based on the traversal order.

The system calls the completion handler after it successfully evicts all items, or immediately when an error occurs. Eviction might fail with the following errors:

- NSFileProviderError.Code.unsyncedEdits if the item had nonuploaded changes.

- NSFileProviderError.Code.nonEvictable if the user has marked the item as nonevictable.

- `EBUSY` if the item has open file descriptors on it.

- `EMLINK` if the item has too many hardlinks.

- Other NSPOSIXErrorDomain error codes if the system can’t access or manipulate the corresponding file.

## See Also

### Working with items

func reimportItems(below: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Tells the system to reimport the item and its content recursively.

func requestDownloadForItem(withIdentifier: NSFileProviderItemIdentifier, requestedRange: NSRange?) async throws

func requestDownloadForItem(withIdentifier: NSFileProviderItemIdentifier, requestedRange: NSRange?, completionHandler: ((any Error)?) -> Void)

func requestModification(of: NSFileProviderItemFields, forItemWithIdentifier: NSFileProviderItemIdentifier, options: NSFileProviderModifyItemOptions, completionHandler: ((any Error)?) -> Void)

func enumeratorForMaterializedItems() -> any NSFileProviderEnumerator

Returns an enumerator for all the items the system currently stores on disk.

func enumeratorForPendingItems() -> any NSFileProviderPendingSetEnumerator

Returns an enumerator for the set of pending items.

