

- Safari Services
- SFSafariTab
-  getPagesWithCompletionHandler(\_:) 

Instance Method

# getPagesWithCompletionHandler(\_:)

Calls the completion handler with all of the tab’s active and preloading pages.

macOS 10.12+

``` source
func getPagesWithCompletionHandler(_ completionHandler: @escaping ([SFSafariPage]?) -> Void)
```

``` source
func pages() async -> [SFSafariPage]?
```

## Parameters 

`completionHandler`  

A block to call when the tab’s pages are retrieved.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func pages() async -> [SFSafariPage]?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The tab’s pages include the active page and other pages that Safari might be loading in the background; for example, Top Hits.

## See Also

### Accessing Pages

func getActivePage(completionHandler: (SFSafariPage?) -> Void)

Calls the completion handler passing the active page in the tab.

