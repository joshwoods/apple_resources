

- Safari Services
- SFSafariWindow
-  getAllTabs(completionHandler:) 

Instance Method

# getAllTabs(completionHandler:)

macOS 10.14.4+

``` source
func getAllTabs(completionHandler: @escaping ([SFSafariTab]) -> Void)
```

``` source
func allTabs() async -> [SFSafariTab]
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func allTabs() async -> [SFSafariTab]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Instance Methods

func close()

