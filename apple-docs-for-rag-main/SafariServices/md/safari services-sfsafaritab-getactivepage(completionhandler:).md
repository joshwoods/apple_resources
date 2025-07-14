

- Safari Services
- SFSafariTab
-  getActivePage(completionHandler:) 

Instance Method

# getActivePage(completionHandler:)

Calls the completion handler passing the active page in the tab.

macOS 10.12+

``` source
func getActivePage(completionHandler: @escaping (SFSafariPage?) -> Void)
```

``` source
func activePage() async -> SFSafariPage?
```

## Parameters 

`completionHandler`  

A block to call when the active page is retrieved.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func activePage() async -> SFSafariPage?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Accessing Pages

func getPagesWithCompletionHandler(([SFSafariPage]?) -> Void)

Calls the completion handler with all of the tab’s active and preloading pages.

