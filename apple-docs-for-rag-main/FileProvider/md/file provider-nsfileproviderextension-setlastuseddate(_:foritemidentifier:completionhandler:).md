

- File Provider
- NSFileProviderExtension
-  setLastUsedDate(\_:forItemIdentifier:completionHandler:) 

Instance Method

# setLastUsedDate(\_:forItemIdentifier:completionHandler:)

Marks an item as recently used and sets its relative order in the Recents list.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
func setLastUsedDate(
    _ lastUsedDate: Date?,
    forItemIdentifier itemIdentifier: NSFileProviderItemIdentifier,
    completionHandler: @escaping (NSFileProviderItem?, (any Error)?) -> Void
)
```

``` source
func setLastUsedDate(
    _ lastUsedDate: Date?,
    forItemIdentifier itemIdentifier: NSFileProviderItemIdentifier
) async throws -> NSFileProviderItem
```

## Parameters 

`lastUsedDate`  

The date and time when the item was last used. This value is used as the sort key for the Recents list.

`itemIdentifier`  

The item’s persistent identifier.

`completionHandler`  

A block that takes the following parameters:

`recentlyUsedItem`  
A file provider item that represents the changed item, or `nil` if an error occurred.

`error`  
An error object. If an error occurs, pass in an object that describes the error; otherwise, set it to `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setLastUsedDate(_ lastUsedDate: Date?, forItemIdentifier itemIdentifier: NSFileProviderItemIdentifier) async throws -> NSFileProviderItem
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method is called after the item is accessed by the host app. Override this method to make any necessary local changes. Your implementation should return immediately. Call the completion handler before performing any network activity or other long-running tasks. Defer these tasks to the background.

The `recentlyUsedItem` instance that you pass to the completion handler should match the item’s old file provider item, with only one change: set the item’s lastUsedDate property with the value of the `lastUsedDate` parameter

Always include Items with a non-`nil` lastUsedDate property in your File Provider extension’s working set.

The error parameter is used only for debugging purposes. The error is logged but not shown to the user.

## See Also

### Handling actions

Providing support for user-driven actions

Override methods to handle user-initiated actions.

func createDirectory(withName: String, inParentItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Creates a directory with the given name inside the given parent directory.

func deleteItem(withIdentifier: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Permanently deletes an item from the trash.

func importDocument(at: URL, toParentItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Imports a file or package into the given parent directory.

func renameItem(withIdentifier: NSFileProviderItemIdentifier, toName: String, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Renames a document or directory.

func reparentItem(withIdentifier: NSFileProviderItemIdentifier, toParentItemWithIdentifier: NSFileProviderItemIdentifier, newName: String?, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Moves the specified item into the given parent directory.

func setFavoriteRank(NSNumber?, forItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Marks a directory as a favorite and sets its relative order in the Favorites list.

func setTagData(Data?, forItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Tags an item.

func trashItem(withIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Moves an item into the trash.

func untrashItem(withIdentifier: NSFileProviderItemIdentifier, toParentItemIdentifier: NSFileProviderItemIdentifier?, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Moves an item out of the trash.

