

- Matter
- MTRXPCServerProtocol_MTRDevice
-  deviceController(\_:nodeID:writeAttributeWithEndpointID:clusterID:attributeID:value:expectedValueInterval:timedWriteTimeout:) 

Instance Method

# deviceController(\_:nodeID:writeAttributeWithEndpointID:clusterID:attributeID:value:expectedValueInterval:timedWriteTimeout:)

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    writeAttributeWithEndpointID endpointID: NSNumber,
    clusterID: NSNumber,
    attributeID: NSNumber,
    value: Any,
    expectedValueInterval: NSNumber?,
    timedWriteTimeout timeout: NSNumber?
)
```

**Required**

