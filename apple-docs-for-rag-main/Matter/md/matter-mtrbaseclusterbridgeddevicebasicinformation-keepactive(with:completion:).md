

- Matter
- MTRBaseClusterBridgedDeviceBasicInformation
-  keepActive(with:completion:) 

Instance Method

# keepActive(with:completion:)

Command KeepActive

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func keepActive(
    with params: MTRBridgedDeviceBasicInformationClusterKeepActiveParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func keepActive(with params: MTRBridgedDeviceBasicInformationClusterKeepActiveParams) async throws
```

## Discussion

The server SHALL attempt to keep the devices specified active for StayActiveDuration milliseconds when they are next active.

