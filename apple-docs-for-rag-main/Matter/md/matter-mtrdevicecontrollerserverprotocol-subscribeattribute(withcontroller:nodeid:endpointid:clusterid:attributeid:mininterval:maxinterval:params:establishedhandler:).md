

- Matter
- MTRDeviceControllerServerProtocol
-  subscribeAttribute(withController:nodeId:endpointId:clusterId:attributeId:minInterval:maxInterval:params:establishedHandler:) 

Instance Method

# subscribeAttribute(withController:nodeId:endpointId:clusterId:attributeId:minInterval:maxInterval:params:establishedHandler:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.1+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func subscribeAttribute(
    withController controller: Any?,
    nodeId: UInt64,
    endpointId: NSNumber?,
    clusterId: NSNumber?,
    attributeId: NSNumber?,
    minInterval: NSNumber,
    maxInterval: NSNumber,
    params: [String : Any]?,
    establishedHandler: @escaping () -> Void
)
```

**Required**

