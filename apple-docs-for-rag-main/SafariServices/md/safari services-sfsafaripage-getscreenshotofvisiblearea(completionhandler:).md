

- Safari Services
- SFSafariPage
-  getScreenshotOfVisibleArea(completionHandler:) 

Instance Method

# getScreenshotOfVisibleArea(completionHandler:)

macOS 10.14.4+

``` source
func getScreenshotOfVisibleArea(completionHandler: @escaping (NSImage?) -> Void)
```

``` source
func screenshotOfVisibleArea() async -> NSImage?
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func screenshotOfVisibleArea() async -> NSImage?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Instance Methods

func getContainingTab(completionHandler: (SFSafariTab) -> Void)

