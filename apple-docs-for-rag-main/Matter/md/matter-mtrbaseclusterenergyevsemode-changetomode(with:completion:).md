

- Matter
- MTRBaseClusterEnergyEVSEMode
-  changeToMode(with:completion:) 

Instance Method

# changeToMode(with:completion:)

Command ChangeToMode

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func changeToMode(
    with params: MTREnergyEVSEModeClusterChangeToModeParams,
    completion: @escaping (MTREnergyEVSEModeClusterChangeToModeResponseParams?, (any Error)?) -> Void
)
```

``` source
func changeToMode(with params: MTREnergyEVSEModeClusterChangeToModeParams) async throws -> MTREnergyEVSEModeClusterChangeToModeResponseParams
```

## Discussion

This command is used to change device modes.

