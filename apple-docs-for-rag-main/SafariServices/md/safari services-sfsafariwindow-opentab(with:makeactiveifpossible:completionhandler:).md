

- Safari Services
- SFSafariWindow
-  openTab(with:makeActiveIfPossible:completionHandler:) 

Instance Method

# openTab(with:makeActiveIfPossible:completionHandler:)

Opens a tab at the end of the tab bar.

macOS 10.12+

``` source
func openTab(
    with url: URL,
    makeActiveIfPossible activateTab: Bool,
    completionHandler: ((SFSafariTab?) -> Void)? = nil
)
```

``` source
func openTab(
    with url: URL,
    makeActiveIfPossible activateTab: Bool
) async -> SFSafariTab?
```

## Parameters 

`url`  

The URL to navigate to.

`activateTab`  

true to make the tab active; otherwise false.

`completionHandler`  

A block called after the tab is opened.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func openTab(with url: URL, makeActiveIfPossible activateTab: Bool) async -> SFSafariTab?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

If the extension cannot access the URL, no tab is opened.

## See Also

### Working with Tabs

func getActiveTab(completionHandler: (SFSafariTab?) -> Void)

Calls the completion handler with the active tab in the target window.

