

- File Provider
- NSFileProviderReplicatedExtension
-  materializedItemsDidChange(completionHandler:) 

Instance Method

# materializedItemsDidChange(completionHandler:)

Tells the file provider that the set of materialized items changed.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
optional func materializedItemsDidChange(completionHandler: @escaping () -> Void)
```

``` source
optional func materializedItemsDidChange() async
```

## Parameters 

`completionHandler`  

A block that you call after you finish processing the changes.

## Mentioned in 

Synchronizing the File Provider Extension

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func materializedItemsDidChange() async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The system calls this method when the set of materialized items changes, such as when the system downloads the content of a dataless item, or deletes the contents of a materialized item.

Note

The system doesn’t call this method when the item’s content changes.

Keep track of the items in the working set—the set of items that the system has downloaded and is managing on disk—to optimize updates. Your file provider must let the system know about any changes to the working set. If you don’t track the working set, then you need to let the system know about any changes to any items in the remote storage.

For more information, see Synchronizing the File Provider Extension.

