

- Safari Services
- SFSafariPage
-  getContainingTab(completionHandler:) 

Instance Method

# getContainingTab(completionHandler:)

macOS 10.14.4+

``` source
func getContainingTab(completionHandler: @escaping (SFSafariTab) -> Void)
```

``` source
func containingTab() async -> SFSafariTab
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func containingTab() async -> SFSafariTab
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Instance Methods

func getScreenshotOfVisibleArea(completionHandler: (NSImage?) -> Void)

