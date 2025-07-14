

- Safari Services
- SFSafariWindow
-  getToolbarItem(completionHandler:) 

Instance Method

# getToolbarItem(completionHandler:)

Gets the extension’s toolbar item from the target window.

macOS 10.12+

``` source
func getToolbarItem(completionHandler: @escaping (SFSafariToolbarItem?) -> Void)
```

``` source
func toolbarItem() async -> SFSafariToolbarItem?
```

## Parameters 

`completionHandler`  

A block called after the toolbar item is retrieved.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func toolbarItem() async -> SFSafariToolbarItem?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

