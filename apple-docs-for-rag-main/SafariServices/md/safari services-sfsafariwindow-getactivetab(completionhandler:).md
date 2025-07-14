

- Safari Services
- SFSafariWindow
-  getActiveTab(completionHandler:) 

Instance Method

# getActiveTab(completionHandler:)

Calls the completion handler with the active tab in the target window.

macOS 10.12+

``` source
func getActiveTab(completionHandler: @escaping (SFSafariTab?) -> Void)
```

``` source
func activeTab() async -> SFSafariTab?
```

## Parameters 

`completionHandler`  

A block called after the active tab is retrieved.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func activeTab() async -> SFSafariTab?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Working with Tabs

func openTab(with: URL, makeActiveIfPossible: Bool, completionHandler: ((SFSafariTab?) -> Void)?)

Opens a tab at the end of the tab bar.

