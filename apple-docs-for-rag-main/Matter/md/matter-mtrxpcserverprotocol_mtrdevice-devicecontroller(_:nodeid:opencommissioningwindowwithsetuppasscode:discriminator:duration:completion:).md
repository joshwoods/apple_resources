

- Matter
- MTRXPCServerProtocol_MTRDevice
-  deviceController(\_:nodeID:openCommissioningWindowWithSetupPasscode:discriminator:duration:completion:) 

Instance Method

# deviceController(\_:nodeID:openCommissioningWindowWithSetupPasscode:discriminator:duration:completion:)

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    openCommissioningWindowWithSetupPasscode setupPasscode: NSNumber,
    discriminator: NSNumber,
    duration: NSNumber,
    completion: @escaping MTRDeviceOpenCommissioningWindowHandler
)
```

``` source
func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    openCommissioningWindowWithSetupPasscode setupPasscode: NSNumber,
    discriminator: NSNumber,
    duration: NSNumber
) async throws -> MTRSetupPayload
```

**Required**

