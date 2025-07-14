

- Matter
- MTRBaseDevice
-  writeAttribute(withEndpointID:clusterID:attributeID:value:timedWriteTimeout:queue:completion:) 

Instance Method

# writeAttribute(withEndpointID:clusterID:attributeID:value:timedWriteTimeout:queue:completion:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func writeAttribute(
    withEndpointID endpointID: NSNumber,
    clusterID: NSNumber,
    attributeID: NSNumber,
    value: Any,
    timedWriteTimeout timeoutMs: NSNumber?,
    queue: dispatch_queue_t,
    completion: @escaping MTRDeviceResponseHandler
)
```

``` source
func writeAttribute(
    withEndpointID endpointID: NSNumber,
    clusterID: NSNumber,
    attributeID: NSNumber,
    value: Any,
    timedWriteTimeout timeoutMs: NSNumber?,
    queue: dispatch_queue_t
) async throws -> [[String : Any]]
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func writeAttribute(withEndpointID endpointID: NSNumber, clusterID: NSNumber, attributeID: NSNumber, value: Any, timedWriteTimeout timeoutMs: NSNumber?, queue: dispatch_queue_t) async throws -> [[String : Any]]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

