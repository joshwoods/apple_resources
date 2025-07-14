

- Matter
- MTRBaseClusterICDManagement
-  stayActiveRequest(with:completion:) 

Instance Method

# stayActiveRequest(with:completion:)

Command StayActiveRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func stayActiveRequest(
    with params: MTRICDManagementClusterStayActiveRequestParams,
    completion: @escaping (MTRICDManagementClusterStayActiveResponseParams?, (any Error)?) -> Void
)
```

``` source
func stayActiveRequest(with params: MTRICDManagementClusterStayActiveRequestParams) async throws -> MTRICDManagementClusterStayActiveResponseParams
```

## Discussion

Request the end device to stay in Active Mode for an additional ActiveModeThreshold

