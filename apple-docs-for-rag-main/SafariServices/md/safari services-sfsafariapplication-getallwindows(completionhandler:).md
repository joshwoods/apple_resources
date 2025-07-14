

- Safari Services
- SFSafariApplication
-  getAllWindows(completionHandler:) 

Type Method

# getAllWindows(completionHandler:)

macOS 10.14.4+

``` source
class func getAllWindows(completionHandler: @escaping ([SFSafariWindow]) -> Void)
```

``` source
class func allWindows() async -> [SFSafariWindow]
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func allWindows() async -> [SFSafariWindow]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Type Methods

class func getHostApplication(completionHandler: (NSRunningApplication) -> Void)

