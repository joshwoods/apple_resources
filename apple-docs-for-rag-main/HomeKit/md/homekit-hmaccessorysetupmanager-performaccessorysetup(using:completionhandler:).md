

- HomeKit
- HMAccessorySetupManager
-  performAccessorySetup(using:completionHandler:) 

Instance Method

# performAccessorySetup(using:completionHandler:)

Performs the process of setting up accessories with Apple Home.

iOS 15.4+iPadOS 15.4+

``` source
func performAccessorySetup(
    using request: HMAccessorySetupRequest,
    completionHandler completion: @escaping (HMAccessorySetupResult?, (any Error)?) -> Void
)
```

``` source
func performAccessorySetup(using request: HMAccessorySetupRequest) async throws -> HMAccessorySetupResult
```

## Parameters 

`request`  

The accessory setup request.

`completion`  

A block that the framework invokes once the setup process completes.

## Discussion

During the setup process, the framework adds each accessory to a home, assigns it to a room, and provides further configuration based on its services.

