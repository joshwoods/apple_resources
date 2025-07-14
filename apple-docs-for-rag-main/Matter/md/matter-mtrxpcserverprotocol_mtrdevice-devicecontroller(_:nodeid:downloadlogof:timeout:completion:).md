

- Matter
- MTRXPCServerProtocol_MTRDevice
-  deviceController(\_:nodeID:downloadLogOf:timeout:completion:) 

Instance Method

# deviceController(\_:nodeID:downloadLogOf:timeout:completion:)

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
optional func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    downloadLogOf type: MTRDiagnosticLogType,
    timeout: TimeInterval,
    completion: @escaping (URL?, (any Error)?) -> Void
)
```

``` source
optional func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    downloadLogOf type: MTRDiagnosticLogType,
    timeout: TimeInterval
) async throws -> URL
```

