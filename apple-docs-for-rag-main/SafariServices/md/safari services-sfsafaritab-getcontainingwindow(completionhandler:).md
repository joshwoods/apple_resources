

- Safari Services
- SFSafariTab
-  getContainingWindow(completionHandler:) 

Instance Method

# getContainingWindow(completionHandler:)

macOS 10.14.4+

``` source
func getContainingWindow(completionHandler: @escaping (SFSafariWindow?) -> Void)
```

``` source
func containingWindow() async -> SFSafariWindow?
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func containingWindow() async -> SFSafariWindow?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Instance Methods

func close()

func navigate(to: URL)

