

- File Provider
- NSFileProviderReplicatedExtension
-  modifyItem(\_:baseVersion:changedFields:contents:options:request:completionHandler:) 

Instance Method

# modifyItem(\_:baseVersion:changedFields:contents:options:request:completionHandler:)

Tells the file provider that an item’s content or metadata changed.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func modifyItem(
    _ item: NSFileProviderItem,
    baseVersion version: NSFileProviderItemVersion,
    changedFields: NSFileProviderItemFields,
    contents newContents: URL?,
    options: NSFileProviderModifyItemOptions = [],
    request: NSFileProviderRequest,
    completionHandler: @escaping (NSFileProviderItem?, NSFileProviderItemFields, Bool, (any Error)?) -> Void
) -> Progress
```

**Required**

## Parameters 

`item`  

The item to modify.

`version`  

The item’s version.

`changedFields`  

The fields that have changed.

`newContents`  

A URL for the local copy of the item’s new contents.

`options`  

The modification options.

`request`  

An object that identifies the context of that request, such as the requesting app.

`completionHandler`  

A block that you call after uploading the changes to your remote storage. You pass the following parameters:

`item`  
The newly modified item.

`stillPendingFields`  
Any fields that you haven’t yet applied. If you can apply all the fields at once, pass an empty `NSFileProviderItemField` instance.

`shouldFetchContent`  
A Boolean value that indicates whether the system should fetch the item’s content from your remote storage.

`error`  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Return Value

An item that tracks your extension’s progress.

## Discussion

The system calls this method when the user modifies an item—for example, moving it, renaming it, or updating its content. The `changedFields` parameter may contain multiple items, indicating that multiple changes have occurred. Update the version of the item in your remote storage to match, and then call the callback handler.

## See Also

### Managing Items

func createItem(basedOn: NSFileProviderItem, fields: NSFileProviderItemFields, contents: URL?, options: NSFileProviderCreateItemOptions, request: NSFileProviderRequest, completionHandler: (NSFileProviderItem?, NSFileProviderItemFields, Bool, (any Error)?) -> Void) -> Progress

Tells the file provider to create or import an item based on a template.

**Required**

struct NSFileProviderCreateItemOptions

Options for creating items.

struct NSFileProviderModifyItemOptions

Options for modifying items.

func deleteItem(identifier: NSFileProviderItemIdentifier, baseVersion: NSFileProviderItemVersion, options: NSFileProviderDeleteItemOptions, request: NSFileProviderRequest, completionHandler: ((any Error)?) -> Void) -> Progress

Tells the file provider to delete an item forever.

**Required**

struct NSFileProviderDeleteItemOptions

Options for deleting items.

