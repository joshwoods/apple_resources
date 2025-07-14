

- Foundation
- NSFilePresenter
-  primaryPresentedItemURL 

Instance Property

# primaryPresentedItemURL

The URL of a secondary item’s primary presented file or directory.

macOS 10.8+

``` source
optional var primaryPresentedItemURL: URL? { get }
```

## Discussion

This property supports App Sandbox in macOS.

Some apps require access to secondary files or directories with names that are related to the primary, user-selected file. For example, a subtitle file, by convention, has the same name as its corresponding movie file, but with a different filename extension. If a movie player is sandboxed, an NSOpenPanel object will grant access only to the user-selected movie file (the primary item) and not its associated subtitle file (the secondary item).

To gain access to a secondary item, first register an NSFilePresenter object for it. At any point in its existence, a secondary item must be able to return an NSURL object to its primary item. This is done by using this property. When done accessing the secondary item, unregister the file presenter object.

## See Also

### Accessing File Presenter Attributes

var presentedItemURL: URL?

The URL of the presented file or directory.

**Required**

var presentedItemOperationQueue: OperationQueue

The operation queue in which to execute presenter-related messages.

**Required**

