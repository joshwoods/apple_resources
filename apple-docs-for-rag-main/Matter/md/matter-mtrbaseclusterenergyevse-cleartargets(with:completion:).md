

- Matter
- MTRBaseClusterEnergyEVSE
-  clearTargets(with:completion:) 

Instance Method

# clearTargets(with:completion:)

Command ClearTargets

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func clearTargets(
    with params: MTREnergyEVSEClusterClearTargetsParams?,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func clearTargets(with params: MTREnergyEVSEClusterClearTargetsParams?) async throws
```

## Discussion

Allows a client to clear all stored charging targets.

