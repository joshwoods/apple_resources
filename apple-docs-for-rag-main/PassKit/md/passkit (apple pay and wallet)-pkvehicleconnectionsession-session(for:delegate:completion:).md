

- PassKit (Apple Pay and Wallet)
- PKVehicleConnectionSession
-  session(for:delegate:completion:) 

Type Method

# session(for:delegate:completion:)

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOSvisionOS 1.0+watchOS 8.5+

``` source
class func session(
    for pass: PKSecureElementPass,
    delegate: any PKVehicleConnectionDelegate,
    completion: @escaping (PKVehicleConnectionSession?, (any Error)?) -> Void
)
```

``` source
class func session(
    for pass: PKSecureElementPass,
    delegate: any PKVehicleConnectionDelegate
) async throws -> PKVehicleConnectionSession
```

