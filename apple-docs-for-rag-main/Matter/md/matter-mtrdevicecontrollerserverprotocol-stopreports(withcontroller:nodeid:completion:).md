

- Matter
- MTRDeviceControllerServerProtocol
-  stopReports(withController:nodeId:completion:) 

Instance Method

# stopReports(withController:nodeId:completion:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.1+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func stopReports(
    withController controller: Any?,
    nodeId: UInt64,
    completion: @escaping () -> Void
)
```

``` source
func stopReports(
    withController controller: Any?,
    nodeId: UInt64
) async
```

**Required**

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func stopReports(withController controller: Any?, nodeId: UInt64) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

