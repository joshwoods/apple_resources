

- Execution Policy
- EPDeveloperTool
-  requestAccess(completionHandler:) 

Instance Method

# requestAccess(completionHandler:)

Mac Catalyst 13.0+macOS 10.15+

``` source
func requestAccess(completionHandler handler: @escaping (Bool) -> Void)
```

``` source
func requestAccess() async -> Bool
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

