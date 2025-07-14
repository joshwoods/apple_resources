

- File Provider
- NSFileProviderCreateItemOptions
-  mayAlreadyExist 

Type Property

# mayAlreadyExist

An option indicating that the item may already exist in your remote storage.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
static var mayAlreadyExist: NSFileProviderCreateItemOptions { get }
```

## Discussion

Your extension should examine the item and determine whether it exists in your remote storage. Because the system may try to reimport a large number of items at once, avoid performing any computationally expensive tasks while trying to match items.

The system attempts to create an item using this flag in the following situations:

- The system reimports its items after an action that might cause it to lose synchronization with your remote storage, such as when restoring a backup or migrating to a new device.

- When merging two directories, the system attempts to create each child object passing the mayAlreadyExist flag. Your extension can then recursively merge the child items.

After processing all the imported items, the system calls the importDidFinish(completionHandler:) method.

## See Also

### Choosing Create Item Options

static var deletionConflicted: NSFileProviderCreateItemOptions

A value indicating a conflict for a deleted item.

