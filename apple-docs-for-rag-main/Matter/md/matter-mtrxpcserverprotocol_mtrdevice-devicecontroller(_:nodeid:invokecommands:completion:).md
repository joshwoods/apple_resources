

- Matter
- MTRXPCServerProtocol_MTRDevice
-  deviceController(\_:nodeID:invokeCommands:completion:) 

Instance Method

# deviceController(\_:nodeID:invokeCommands:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
optional func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    invokeCommands commands: [[MTRCommandWithRequiredResponse]],
    completion: @escaping MTRDeviceResponseHandler
)
```

``` source
optional func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    invokeCommands commands: [[MTRCommandWithRequiredResponse]]
) async throws -> [[String : Any]]
```

