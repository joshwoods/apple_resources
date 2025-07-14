

- File Provider
- NSFileProviderCreateItemOptions
-  deletionConflicted 

Type Property

# deletionConflicted

A value indicating a conflict for a deleted item.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
static var deletionConflicted: NSFileProviderCreateItemOptions { get }
```

## Discussion

If the File Provider extension signals the deletion of an item but the deletion conflicts with local edits, the system attempts to create the modified item by calling the createItem(basedOn:fields:contents:options:request:completionHandler:) method, and passing this value as an option.

## See Also

### Choosing Create Item Options

static var mayAlreadyExist: NSFileProviderCreateItemOptions

An option indicating that the item may already exist in your remote storage.

