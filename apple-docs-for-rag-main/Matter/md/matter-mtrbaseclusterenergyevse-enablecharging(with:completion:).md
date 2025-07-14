

- Matter
- MTRBaseClusterEnergyEVSE
-  enableCharging(with:completion:) 

Instance Method

# enableCharging(with:completion:)

Command EnableCharging

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func enableCharging(
    with params: MTREnergyEVSEClusterEnableChargingParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func enableCharging(with params: MTREnergyEVSEClusterEnableChargingParams) async throws
```

## Discussion

This command allows a client to enable the EVSE to charge an EV, and to provide or update the maximum and minimum charge current.

