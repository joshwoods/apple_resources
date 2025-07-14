

- Safari Services
- SFSafariApplication
-  getHostApplication(completionHandler:) 

Type Method

# getHostApplication(completionHandler:)

macOS 10.13+

``` source
class func getHostApplication(completionHandler: @escaping (NSRunningApplication) -> Void)
```

``` source
class func hostApplication() async -> NSRunningApplication
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func hostApplication() async -> NSRunningApplication
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Type Methods

class func getAllWindows(completionHandler: ([SFSafariWindow]) -> Void)

