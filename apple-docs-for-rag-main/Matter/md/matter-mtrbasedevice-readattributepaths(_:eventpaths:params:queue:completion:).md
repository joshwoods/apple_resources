

- Matter
- MTRBaseDevice
-  readAttributePaths(\_:eventPaths:params:queue:completion:) 

Instance Method

# readAttributePaths(\_:eventPaths:params:queue:completion:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func readAttributePaths(
    _ attributePaths: [MTRAttributeRequestPath]?,
    eventPaths: [MTREventRequestPath]?,
    params: MTRReadParams?,
    queue: dispatch_queue_t,
    completion: @escaping MTRDeviceResponseHandler
)
```

``` source
func readAttributePaths(
    _ attributePaths: [MTRAttributeRequestPath]?,
    eventPaths: [MTREventRequestPath]?,
    params: MTRReadParams?,
    queue: dispatch_queue_t
) async throws -> [[String : Any]]
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func readAttributePaths(_ attributePaths: [MTRAttributeRequestPath]?, eventPaths: [MTREventRequestPath]?, params: MTRReadParams?, queue: dispatch_queue_t) async throws -> [[String : Any]]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

