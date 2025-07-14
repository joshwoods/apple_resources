

- File Provider
- Nonreplicated File Provider extension
- NSFileProviderExtension
-  Providing support for user-driven actions 

# Providing support for user-driven actions

Override methods to handle user-initiated actions.

## Overview

When the user performs an action in the document browser (for example, moving, renaming, or deleting an item) the system calls the corresponding method on your NSFileProviderExtension subclass.

The following table shows the action method for each action type:

| User action | Action method |
|----|----|
| Creates a new folder | createDirectory(withName:inParentItemIdentifier:completionHandler:) |
| Deletes a document or folder | deleteItem(withIdentifier:completionHandler:) |
| Imports a document | importDocument(at:toParentItemIdentifier:completionHandler:) |
| Renames a document or folder | renameItem(withIdentifier:toName:completionHandler:) |
| Moves a document or folder | reparentItem(withIdentifier:toParentItemWithIdentifier:newName:completionHandler:) |
| Sets or changes a folder’s favorite rank | setFavoriteRank(_:forItemIdentifier:completionHandler:) |
| Uses a document | setLastUsedDate(_:forItemIdentifier:completionHandler:) |
| Tags or untags a document or folder | setTagData(_:forItemIdentifier:completionHandler:) |
| Moves a document or folder to the trash | trashItem(withIdentifier:completionHandler:) |
| Removes a document or folder from the trash | untrashItem(withIdentifier:toParentItemIdentifier:completionHandler:) |

When the action method is called, ensure that your implementation:

1.  Makes any necessary local changes, including updates to the working set

2.  Schedules a background update for your server

3.  Signals that the changes have occurred

4.  Calls the completion handler with the results

All the action methods are expected to work offline, and should return immediately. Call the completion handler before performing any network activity or other long-running tasks. Defer these tasks to the background.

## Topics

### Signaling Changes

Signaling Changes for User-Driven Actions

Signal the system about any changes created by an action.

### Handling Errors

Handling Errors with User-Driven Actions

Handle any errors that occur while processing the action.

## See Also

### Handling actions

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

func setLastUsedDate(Date?, forItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Marks an item as recently used and sets its relative order in the Recents list.

func setTagData(Data?, forItemIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Tags an item.

func trashItem(withIdentifier: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Moves an item into the trash.

func untrashItem(withIdentifier: NSFileProviderItemIdentifier, toParentItemIdentifier: NSFileProviderItemIdentifier?, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void)

Moves an item out of the trash.

