

- Matter
- MTRBaseClusterLaundryWasherMode
-  changeToMode(with:completion:) 

Instance Method

# changeToMode(with:completion:)

Command ChangeToMode

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func changeToMode(
    with params: MTRLaundryWasherModeClusterChangeToModeParams,
    completion: @escaping (MTRLaundryWasherModeClusterChangeToModeResponseParams?, (any Error)?) -> Void
)
```

``` source
func changeToMode(with params: MTRLaundryWasherModeClusterChangeToModeParams) async throws -> MTRLaundryWasherModeClusterChangeToModeResponseParams
```

## Discussion

This command is used to change device modes. On receipt of this command the device SHALL respond with a ChangeToModeResponse command.

