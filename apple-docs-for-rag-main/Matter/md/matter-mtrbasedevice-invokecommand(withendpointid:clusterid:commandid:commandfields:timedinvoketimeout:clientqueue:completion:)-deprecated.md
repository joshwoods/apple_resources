

- Matter
- MTRBaseDevice
-  invokeCommand(withEndpointId:clusterId:commandId:commandFields:timedInvokeTimeout:clientQueue:completion:) Deprecated

Instance Method

# invokeCommand(withEndpointId:clusterId:commandId:commandFields:timedInvokeTimeout:clientQueue:completion:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func invokeCommand(
    withEndpointId endpointId: NSNumber,
    clusterId: NSNumber,
    commandId: NSNumber,
    commandFields: Any,
    timedInvokeTimeout timeoutMs: NSNumber?,
    clientQueue: dispatch_queue_t,
    completion: @escaping MTRDeviceResponseHandler
)
```

``` source
func invokeCommand(
    withEndpointId endpointId: NSNumber,
    clusterId: NSNumber,
    commandId: NSNumber,
    commandFields: Any,
    timedInvokeTimeout timeoutMs: NSNumber?,
    clientQueue: dispatch_queue_t
) async throws -> [[String : Any]]
```

Deprecated

Please use invokeCommandWithEndpointID:clusterID:commandID:commandFields:timedInvokeTimeout:queue:completion

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func invokeCommand(withEndpointId endpointId: NSNumber, clusterId: NSNumber, commandId: NSNumber, commandFields: Any, timedInvokeTimeout timeoutMs: NSNumber?, clientQueue: dispatch_queue_t) async throws -> [[String : Any]]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

