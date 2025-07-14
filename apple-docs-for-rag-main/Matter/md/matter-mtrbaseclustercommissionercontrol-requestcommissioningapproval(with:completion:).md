

- Matter
- MTRBaseClusterCommissionerControl
-  requestCommissioningApproval(with:completion:) 

Instance Method

# requestCommissioningApproval(with:completion:)

Command RequestCommissioningApproval

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func requestCommissioningApproval(
    with params: MTRCommissionerControlClusterRequestCommissioningApprovalParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func requestCommissioningApproval(with params: MTRCommissionerControlClusterRequestCommissioningApprovalParams) async throws
```

## Discussion

This command is sent by a client to request approval for a future CommissionNode call.

