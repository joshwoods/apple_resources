

- File Provider
- NSFileProviderExtension
-  reparentItem(withIdentifier:toParentItemWithIdentifier:newName:completionHandler:) 

Instance Method

# reparentItem(withIdentifier:toParentItemWithIdentifier:newName:completionHandler:)

Moves the specified item into the given parent directory.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
func reparentItem(
    withIdentifier itemIdentifier: NSFileProviderItemIdentifier,
    toParentItemWithIdentifier parentItemIdentifier: NSFileProviderItemIdentifier,
    newName: String?,
    completionHandler: @escaping (NSFileProviderItem?, (any Error)?) -> Void
)
```

``` source
func reparentItem(
    withIdentifier itemIdentifier: NSFileProviderItemIdentifier,
    toParentItemWithIdentifier parentItemIdentifier: NSFileProviderItemIdentifier,
    newName: String?
) async throws -> NSFileProviderItem
```

## Parameters 

`itemIdentifier`  

The item’s persistent identifier.

`parentItemIdentifier`  

The persistent identifier for the new parent directory.

`newName`  

The new name of the file or directory, including the file extension.

`completionHandler`  

A block that takes the following parameters:

`reparentedItem`  
A file provider item that represents the reparented item, or `nil` if an error occurred.

`error`  
An error object. If an error occurs, pass in an object that describes the error; otherwise, set it to `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func reparentItem(withIdentifier itemIdentifier: NSFileProviderItemIdentifier, toParentItemWithIdentifier parentItemIdentifier: NSFileProviderItemIdentifier, newName: String?) async throws -> NSFileProviderItem
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method is called when the user moves a document or directory. Override this method to make any necessary local changes to the item and both its old and new parents. Your implementation should return immediately. Call the completion handler before performing any network activity or other long-running tasks. Defer these tasks to the background.

The `reparentedItem` instance that you pass to the completion handler should match the item’s old file provider item, with only one change: set the parentItemIdentifier property to the value passed to the `parentItemIdentifier` parameter.

The user’s ability to rename an item is controlled by the item’s allowsRenaming capability.

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

func setFavoriteRank(NSNumber?, forItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Marks a directory as a favorite and sets its relative order in the Favorites list.

func setLastUsedDate(Date?, forItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Marks an item as recently used and sets its relative order in the Recents list.

func setTagData(Data?, forItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Tags an item.

func trashItem(withIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Moves an item into the trash.

func untrashItem(withIdentifier: NSFileProviderItemIdentifier, toParentItemIdentifier: NSFileProviderItemIdentifier?, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Moves an item out of the trash.

