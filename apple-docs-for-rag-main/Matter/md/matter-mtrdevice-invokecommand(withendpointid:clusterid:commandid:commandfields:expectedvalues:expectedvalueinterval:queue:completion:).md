

- Matter
- MTRDevice
-  invokeCommand(withEndpointID:clusterID:commandID:commandFields:expectedValues:expectedValueInterval:queue:completion:) 

Instance Method

# invokeCommand(withEndpointID:clusterID:commandID:commandFields:expectedValues:expectedValueInterval:queue:completion:)

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
func invokeCommand(
    withEndpointID endpointID: NSNumber,
    clusterID: NSNumber,
    commandID: NSNumber,
    commandFields: [String : Any]?,
    expectedValues: [[String : Any]]?,
    expectedValueInterval: NSNumber?,
    queue: dispatch_queue_t,
    completion: @escaping MTRDeviceResponseHandler
)
```

``` source
func invokeCommand(
    withEndpointID endpointID: NSNumber,
    clusterID: NSNumber,
    commandID: NSNumber,
    commandFields: [String : Any]?,
    expectedValues: [[String : Any]]?,
    expectedValueInterval: NSNumber?,
    queue: dispatch_queue_t
) async throws -> [[String : Any]]
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func invokeCommand(withEndpointID endpointID: NSNumber, clusterID: NSNumber, commandID: NSNumber, commandFields: [String : Any]?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, queue: dispatch_queue_t) async throws -> [[String : Any]]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

