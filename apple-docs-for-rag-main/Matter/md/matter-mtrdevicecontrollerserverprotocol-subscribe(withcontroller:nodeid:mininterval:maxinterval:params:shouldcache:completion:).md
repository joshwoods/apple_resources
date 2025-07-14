

- Matter
- MTRDeviceControllerServerProtocol
-  subscribe(withController:nodeId:minInterval:maxInterval:params:shouldCache:completion:) 

Instance Method

# subscribe(withController:nodeId:minInterval:maxInterval:params:shouldCache:completion:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.1+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func subscribe(
    withController controller: Any?,
    nodeId: UInt64,
    minInterval: NSNumber,
    maxInterval: NSNumber,
    params: [String : Any]?,
    shouldCache: Bool,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func subscribe(
    withController controller: Any?,
    nodeId: UInt64,
    minInterval: NSNumber,
    maxInterval: NSNumber,
    params: [String : Any]?,
    shouldCache: Bool
) async throws
```

**Required**

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func subscribe(withController controller: Any?, nodeId: UInt64, minInterval: NSNumber, maxInterval: NSNumber, params: [String : Any]?, shouldCache: Bool) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

