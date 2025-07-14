

- Matter
- MTRDevice
-  invokeCommand(withEndpointID:clusterID:commandID:commandFields:expectedValues:expectedValueInterval:timedInvokeTimeout:clientQueue:completion:) Deprecated

Instance Method

# invokeCommand(withEndpointID:clusterID:commandID:commandFields:expectedValues:expectedValueInterval:timedInvokeTimeout:clientQueue:completion:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func invokeCommand(
    withEndpointID endpointID: NSNumber,
    clusterID: NSNumber,
    commandID: NSNumber,
    commandFields: Any,
    expectedValues: [[String : Any]]?,
    expectedValueInterval: NSNumber?,
    timedInvokeTimeout timeout: NSNumber?,
    clientQueue queue: dispatch_queue_t,
    completion: @escaping MTRDeviceResponseHandler
)
```

``` source
func invokeCommand(
    withEndpointID endpointID: NSNumber,
    clusterID: NSNumber,
    commandID: NSNumber,
    commandFields: Any,
    expectedValues: [[String : Any]]?,
    expectedValueInterval: NSNumber?,
    timedInvokeTimeout timeout: NSNumber?,
    clientQueue queue: dispatch_queue_t
) async throws -> [[String : Any]]
```

Deprecated

Please use invokeCommandWithEndpointID:clusterID:commandID:commandFields:expectedValues:expectedValueInterval:timedInvokeTimeout:queue:completion:

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func invokeCommand(withEndpointID endpointID: NSNumber, clusterID: NSNumber, commandID: NSNumber, commandFields: Any, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, timedInvokeTimeout timeout: NSNumber?, clientQueue queue: dispatch_queue_t) async throws -> [[String : Any]]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

