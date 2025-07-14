

- Matter
- MTRXPCServerProtocol_MTRDevice
-  deviceController(\_:nodeID:readAttributePaths:withReply:) 

Instance Method

# deviceController(\_:nodeID:readAttributePaths:withReply:)

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    readAttributePaths attributePaths: [MTRAttributeRequestPath],
    withReply reply: @escaping ([[String : Any]]) -> Void
)
```

``` source
func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    readAttributePaths attributePaths: [MTRAttributeRequestPath]
) async -> [[String : Any]]
```

**Required**

