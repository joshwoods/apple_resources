

- File Provider
- NSFileProviderReplicatedExtension
-  deleteItem(identifier:baseVersion:options:request:completionHandler:) 

Instance Method

# deleteItem(identifier:baseVersion:options:request:completionHandler:)

Tells the file provider to delete an item forever.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func deleteItem(
    identifier: NSFileProviderItemIdentifier,
    baseVersion version: NSFileProviderItemVersion,
    options: NSFileProviderDeleteItemOptions = [],
    request: NSFileProviderRequest,
    completionHandler: @escaping ((any Error)?) -> Void
) -> Progress
```

**Required**

## Parameters 

`identifier`  

The identifier of the object to delete.

`version`  

The version of the item to delete.

`options`  

The options for deleting the item.

`request`  

An object that identifies the context of that request, such as the requesting app.

`completionHandler`  

A block that you call after deleting the item from your remote storage. You pass the following parameter:

`error`  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Return Value

An item that tracks your extension’s progress.

## Discussion

The system calls this method when the user deletes an item that was already in the trash. Users can only delete items that have the allowsDeleting capability.

Remove the item from the trash and delete it from your remote storage. If the item is in the working set, notify the system about the change by calling signalEnumerator(for:completionHandler:) and passing workingSet for the `containerItemIdentifier` parameter. If the deletion is recursive, be sure to check all the deleted items, and notify the system to any changes in the working set.

If your extension doesn’t recognize the item, you can just report success. The system then removes the local copy of the item.

## See Also

### Managing Items

func createItem(basedOn: NSFileProviderItem, fields: NSFileProviderItemFields, contents: URL?, options: NSFileProviderCreateItemOptions, request: NSFileProviderRequest, completionHandler: (NSFileProviderItem?, NSFileProviderItemFields, Bool, (any Error)?) -> Void) -> Progress

Tells the file provider to create or import an item based on a template.

**Required**

struct NSFileProviderCreateItemOptions

Options for creating items.

func modifyItem(NSFileProviderItem, baseVersion: NSFileProviderItemVersion, changedFields: NSFileProviderItemFields, contents: URL?, options: NSFileProviderModifyItemOptions, request: NSFileProviderRequest, completionHandler: (NSFileProviderItem?, NSFileProviderItemFields, Bool, (any Error)?) -> Void) -> Progress

Tells the file provider that an item’s content or metadata changed.

**Required**

struct NSFileProviderModifyItemOptions

Options for modifying items.

struct NSFileProviderDeleteItemOptions

Options for deleting items.

