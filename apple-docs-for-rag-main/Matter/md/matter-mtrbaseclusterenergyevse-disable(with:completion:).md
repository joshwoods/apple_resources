

- Matter
- MTRBaseClusterEnergyEVSE
-  disable(with:completion:) 

Instance Method

# disable(with:completion:)

Command Disable

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func disable(
    with params: MTREnergyEVSEClusterDisableParams?,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func disable(with params: MTREnergyEVSEClusterDisableParams?) async throws
```

## Discussion

Allows a client to disable the EVSE from charging and discharging.

