

- Matter
- MTRXPCServerProtocol_MTRDeviceController
-  deviceController(\_:getNodesWithStoredDataWithReply:) 

Instance Method

# deviceController(\_:getNodesWithStoredDataWithReply:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
optional func deviceController(
    _ controller: UUID,
    getNodesWithStoredDataWithReply reply: @escaping ([NSNumber]) -> Void
)
```

``` source
optional func deviceControllerGetNodesWithStoredData(_ controller: UUID) async -> [NSNumber]
```

