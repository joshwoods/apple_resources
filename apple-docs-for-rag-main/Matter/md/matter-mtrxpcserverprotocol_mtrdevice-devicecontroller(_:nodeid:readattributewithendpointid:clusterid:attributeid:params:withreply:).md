

- Matter
- MTRXPCServerProtocol_MTRDevice
-  deviceController(\_:nodeID:readAttributeWithEndpointID:clusterID:attributeID:params:withReply:) 

Instance Method

# deviceController(\_:nodeID:readAttributeWithEndpointID:clusterID:attributeID:params:withReply:)

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    readAttributeWithEndpointID endpointID: NSNumber,
    clusterID: NSNumber,
    attributeID: NSNumber,
    params: MTRReadParams?,
    withReply reply: @escaping ([String : Any]?) -> Void
)
```

``` source
func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    readAttributeWithEndpointID endpointID: NSNumber,
    clusterID: NSNumber,
    attributeID: NSNumber,
    params: MTRReadParams?
) async -> [String : Any]?
```

**Required**

