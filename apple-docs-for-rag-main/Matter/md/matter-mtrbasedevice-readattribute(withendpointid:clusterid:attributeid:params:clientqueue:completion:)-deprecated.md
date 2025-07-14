

- Matter
- MTRBaseDevice
-  readAttribute(withEndpointId:clusterId:attributeId:params:clientQueue:completion:) Deprecated

Instance Method

# readAttribute(withEndpointId:clusterId:attributeId:params:clientQueue:completion:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func readAttribute(
    withEndpointId endpointId: NSNumber?,
    clusterId: NSNumber?,
    attributeId: NSNumber?,
    params: MTRReadParams?,
    clientQueue: dispatch_queue_t,
    completion: @escaping MTRDeviceResponseHandler
)
```

``` source
func readAttribute(
    withEndpointId endpointId: NSNumber?,
    clusterId: NSNumber?,
    attributeId: NSNumber?,
    params: MTRReadParams?,
    clientQueue: dispatch_queue_t
) async throws -> [[String : Any]]
```

Deprecated

Please use readAttributesWithEndpointID:clusterID:attributeID:params:queue:completion:

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func readAttribute(withEndpointId endpointId: NSNumber?, clusterId: NSNumber?, attributeId: NSNumber?, params: MTRReadParams?, clientQueue: dispatch_queue_t) async throws -> [[String : Any]]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

