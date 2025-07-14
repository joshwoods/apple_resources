

- Matter
- MTRBaseClusterDeviceEnergyManagement
-  resumeRequest(with:completion:) 

Instance Method

# resumeRequest(with:completion:)

Command ResumeRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func resumeRequest(
    with params: MTRDeviceEnergyManagementClusterResumeRequestParams?,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func resumeRequest(with params: MTRDeviceEnergyManagementClusterResumeRequestParams?) async throws
```

## Discussion

Allows a client to cancel the PauseRequest command and enable earlier resumption of operation.

